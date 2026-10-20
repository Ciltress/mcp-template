# Graph Report - src  (2026-10-20)

## Corpus Check
- Corpus is ~28.644 words - fits in a single context window. You may not need a graph.

## Summary
- 270 nodes · 555 edges · 14 communities detected
- Extraction: 100% EXTRACTED · 0% INFERRED · 0% AMBIGUOUS
- Token cost: 0 input · 0 output
- Edge kinds: contains: 178 · imports: 163 · imports_from: 86 · calls: 63 · method: 50 · re_exports: 8 · inherits: 6 · implements: 1


## Input Scope
- Requested: all
- Resolved: all (source: configured-default)
- Included files: 35 · Candidates: recursive
- Excluded: 0 untracked · 0 ignored · 0 sensitive · 0 missing committed

## Graph Freshness
- Built from Git commit: `8892487`
- Compare this hash to `git rev-parse HEAD` before trusting freshness-sensitive graph output.
## God Nodes (most connected - your core abstractions)
1. `AppServer` - 22 edges
2. `InMemoryNotesBackend` - 18 edges
3. `AppBackend` - 13 edges
4. `NoteStore` - 12 edges
5. `NotesHandlers` - 11 edges
6. `ToolDefinition` - 10 edges
7. `createHandlers()` - 9 edges
8. `discoverSkills()` - 7 edges
9. `PermanentBackendError` - 6 edges
10. `DocsHandlers` - 6 edges

## Surprising Connections (you probably didn't know these)
- `InMemoryNotesBackend` --implements--> `NotesBackend`  [EXTRACTED]
  backend/notes.ts → backend/notes.ts  _Bridges community 4 → community 9_

## Communities

### Community 0 - "Community 0"
Cohesion: 0.08
Nodes (24): AppBackend, createHandlers(), evaluateGate(), GATED_FEATURES, GatedFeature, GateResult, gatingEnabled(), cell() (+16 more)

### Community 1 - "Community 1"
Cohesion: 0.12
Nodes (21): ANALYSIS, applyProfile(), CORE_WRITE, GUIDANCE, PROFILE_NAMES, ProfileDefinition, ProfileError, ProfileName (+13 more)

### Community 2 - "Community 2"
Cohesion: 0.12
Nodes (21): REQUIRED_ENV, packageJson, PROJECT_ROOT, RESOURCE_SCHEME, SERVER_INFO, discoverSkills(), findSkill(), parseFrontmatter() (+13 more)

### Community 3 - "Community 3"
Cohesion: 0.12
Nodes (19): HERE, server, parseList(), createRateLimiter(), extractBearerToken(), hostAllowed(), normalizeOrigin(), originAllowed() (+11 more)

### Community 4 - "Community 4"
Cohesion: 0.12
Nodes (3): InMemoryNotesBackend, normaliseTags(), NoteStore

### Community 5 - "Community 5"
Cohesion: 0.17
Nodes (8): ToolSpec, BaseHandler, NotesHandlers, optionalString(), optionalTags(), requireString(), BaseHandler, SkillsHandlers

### Community 6 - "Community 6"
Cohesion: 0.21
Nodes (14): BaseHandler, DocsHandlers, extractSection(), guideById(), guideByUri(), GuideDefinition, guideIndex(), GuideNotFoundError (+6 more)

### Community 7 - "Community 7"
Cohesion: 0.16
Nodes (2): AppServer, withTimeout()

### Community 8 - "Community 8"
Cohesion: 0.19
Nodes (9): asMcpError(), envelope(), getMetrics(), handle(), specs(), trackRequest(), createLogger(), Logger (+1 more)

### Community 9 - "Community 9"
Cohesion: 0.15
Nodes (11): Backend, EXAMPLE_NOTES, InMemoryNotesOptions, NewNote, Note, NotePatch, NOTES_FEATURES, NotesBackend (+3 more)

### Community 10 - "Community 10"
Cohesion: 0.32
Nodes (9): Backend, HealthReport, isPermanent(), PermanentBackendError, SessionExpiredError, BackendOptions, createBackend(), setup() (+1 more)

### Community 11 - "Community 11"
Cohesion: 0.23
Nodes (7): DOMAIN_METHODS, fakeBackend(), FakeBackendOptions, LIFECYCLE, recordingBackend(), seedStore(), BASE_ENV

### Community 12 - "Community 12"
Cohesion: 0.32
Nodes (7): ACCEPTED, BASE_ENV, headers(), initializeMessage, openSession(), post(), toolsList

### Community 13 - "Community 13"
Cohesion: 0.60
Nodes (3): AppServer, startServer(), TestableServer

## Knowledge Gaps
- **53 isolated node(s):** `CATALOGUE`, `LIFECYCLE`, `DOMAIN_METHODS`, `SAMPLE`, `Stubs` (+48 more)
  These have ≤1 connection - possible missing edges or undocumented components.
- **Thin community `Community 7`** (2 nodes): `AppServer`, `withTimeout()`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.

## Suggested Questions
_Questions this graph is uniquely positioned to answer:_

- **Why does `AppServer` connect `Community 7` to `Community 3`, `Community 12`, `Community 11`?**
  _High betweenness centrality (0.128) - this node is a cross-community bridge._
- **Why does `InMemoryNotesBackend` connect `Community 4` to `Community 10`, `Community 9`, `Community 11`?**
  _High betweenness centrality (0.091) - this node is a cross-community bridge._
- **Why does `NotesHandlers` connect `Community 5` to `Community 10`?**
  _High betweenness centrality (0.057) - this node is a cross-community bridge._
- **What connects `CATALOGUE`, `LIFECYCLE`, `DOMAIN_METHODS` to the rest of the system?**
  _53 weakly-connected nodes found - possible documentation gaps or missing edges._
- **Should `Community 0` be split into smaller, more focused modules?**
  _Cohesion score 0.08367071524966262 - nodes in this community are weakly interconnected._
- **Should `Community 1` be split into smaller, more focused modules?**
  _Cohesion score 0.12315270935960591 - nodes in this community are weakly interconnected._
- **Should `Community 2` be split into smaller, more focused modules?**
  _Cohesion score 0.1164021164021164 - nodes in this community are weakly interconnected._