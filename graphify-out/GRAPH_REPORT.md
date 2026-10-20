# Graph Report - mcp-template  (2026-10-20)

## Corpus Check
- 215 files · ~133,634 words
- Verdict: corpus is large enough that graph structure adds value.
- Unclassified: 11 file(s) not represented in the graph (top: (none) 10, .example 1)

## Summary
- 725 nodes · 1269 edges · 50 communities (34 shown, 16 thin omitted)
- Extraction: 90% EXTRACTED · 10% INFERRED · 0% AMBIGUOUS · INFERRED: 123 edges (avg confidence: 0.82)
- Token cost: 0 input · 0 output

## Community Hubs (Navigation)
- Server Core & SDK
- CI, Agents Guide & Conventions
- Config & Docs Handlers
- Package Manifest
- Skills Repo Changesets
- Learning & Cognition Concepts
- BaseHandler
- Tool Profiles
- Env & HTTP Transport
- Wayfinder & Ticket Mapping
- Doc Generation Script
- In-Memory Notes Backend
- Skills Handlers
- Dev Package & Changesets Tooling
- Template Setup Script
- Writing Skills
- Tests & Fake Backend Helpers
- Skills ADRs & Setup
- Notes Types
- TypeScript Config
- Changesets Config
- Backend Interface
- Ask-Matt & Phase Boundaries
- Git Guardrails & Shoehorn
- Backend Errors
- Registry server.json
- Handoff & Loop Skills
- Fake Backend
- Triage & Agent Briefs
- Domain Docs & TDD
- Deep Module Design
- Research & Merge Skills
- Issue Tracker Setup
- ADR Format & Grilling
- Architecture Improvement
- Prototype Skill
- HITL Loop Script
- Wizard Skill
- Wizard & Handoff Docs
- Wait-What & Agent Writing
- Link Skills Script
- List Skills Script
- Block Dangerous Git
- Teach Skill
- Deprecated Skills
- Architecture openai.yaml
- To-Spec openai.yaml
- Writing Beats openai.yaml

## God Nodes (most connected - your core abstractions)
1. `AppServer` - 31 edges
2. `InMemoryNotesBackend` - 22 edges
3. `BaseHandler` - 22 edges
4. `MCP-Tools guide (how the server behaves)` - 18 edges
5. `AppBackend` - 17 edges
6. `CONTEXT.md (domain glossary)` - 17 edges
7. `NoteStore` - 15 edges
8. `createHandlers()` - 15 edges
9. `ToolDefinition` - 15 edges
10. `Tool router (intent to tool)` - 14 edges

## Surprising Connections (you probably didn't know these)
- `Honest annotations convention` --semantically_similar_to--> `Tool annotations (four hints)`  [INFERRED] [semantically similar]
  AGENTS.md → docs/MCP-Tools.md
- `skills/Development is a submodule, do not edit` --semantically_similar_to--> `Development skills guide`  [INFERRED] [semantically similar]
  AGENTS.md → docs/Development-Skills.md
- `ToolSpec and BaseHandler convention` --semantically_similar_to--> `BaseHandler and ToolSpec execution layer`  [INFERRED] [semantically similar]
  AGENTS.md → docs/MCP-Tools.md
- `Gating (capability gate)` --semantically_similar_to--> `Capability gate (fails open)`  [INFERRED] [semantically similar]
  CONTEXT.md → docs/MCP-Tools.md
- `Profile` --semantically_similar_to--> `Profiles (core, readonly, all)`  [INFERRED] [semantically similar]
  CONTEXT.md → docs/MCP-Tools.md

## Import Cycles
- None detected.

## Hyperedges (group relationships)
- **HTTP request gates in front of a session** — docs_hosting_http_gates, docs_hosting_dns_rebinding, docs_hosting_session_bound_token, docs_hosting_streamable_http [EXTRACTED 1.00]
- **Client adaptation: profiles, response budget, capability gate** — docs_mcp_tools_profiles, docs_mcp_tools_response_budget, docs_mcp_tools_capability_gate, context_client_tier [EXTRACTED 1.00]
- **Guides served at runtime (router, reference, tools, hosting, skills, agents)** — docs_tool_router, docs_tool_reference, docs_mcp_tools, docs_hosting, docs_development_skills, agents [EXTRACTED 1.00]
- **Engineering skill docs pages** — skills_development_docs_engineering_ask_matt, skills_development_docs_engineering_code_review, skills_development_docs_engineering_codebase_design, skills_development_docs_engineering_diagnosing_bugs, skills_development_docs_engineering_domain_modeling, skills_development_docs_engineering_grill_with_docs [INFERRED 0.85]
- **Spec to tickets to implementation flow** — skills_development_docs_engineering_to_spec, skills_development_docs_engineering_to_tickets, skills_development_docs_engineering_implement, skills_development_docs_engineering_tdd [INFERRED 0.85]
- **Main flow: grill, implement, review** — skills_development_skills_engineering_grill_with_docs_skill, skills_development_skills_engineering_implement_skill, skills_development_skills_engineering_code_review_skill, skills_development_skills_engineering_ask_matt_skill [INFERRED 0.85]
- **Issue tracker backends** — skills_development_skills_engineering_setup_matt_pocock_skills_issue_tracker_github_md, skills_development_skills_engineering_setup_matt_pocock_skills_issue_tracker_gitlab_md, skills_development_skills_engineering_setup_matt_pocock_skills_issue_tracker_local_md [INFERRED 0.85]
- **Spec to tickets to implementation flow** — skills_development_skills_engineering_to_tickets_skill, skills_development_skills_in_progress_implement_spec_skill, skills_development_skills_engineering_triage_skill [INFERRED 0.75]
- **Teach workspace state files** — skills_development_skills_productivity_teach_skill, skills_development_skills_productivity_teach_mission_format, skills_development_skills_productivity_teach_resources_format, skills_development_skills_productivity_teach_learning_record_format, skills_development_skills_productivity_teach_glossary_format [EXTRACTED 0.95]
- **User-invoked productivity skills** — skills_development_skills_productivity_teach_skill, skills_development_skills_productivity_to_questionnaire_skill, skills_development_skills_productivity_wait_what_skill [EXTRACTED 0.90]

## Communities (50 total, 16 thin omitted)

### Community 0 - "Server Core & SDK"
Cohesion: 0.07
Nodes (41): @modelcontextprotocol/sdk, AppBackend, ToolSpec, createHandlers(), NotesHandlers, optionalString(), optionalTags(), requireString() (+33 more)

### Community 1 - "CI, Agents Guide & Conventions"
Cohesion: 0.06
Nodes (56): CI workflow (test and build jobs), CI smoke test step (npm run smoke over stdio), AGENTS.md (guidance for agents working on the repo), Starting a new server from the template (7 steps), ToolSpec and BaseHandler convention, CONTEXT.md (domain glossary), Backend, Binding (+48 more)

### Community 2 - "Config & Docs Handlers"
Cohesion: 0.10
Nodes (27): dotenv, REQUIRED_ENV, DocsHandlers, HERE, server, extractSection(), GUIDE_URI_PREFIX, guideById() (+19 more)

### Community 3 - "Package Manifest"
Cohesion: 0.06
Nodes (35): author, bin, mcp-template, dependencies, dotenv, @modelcontextprotocol/sdk, description, devDependencies (+27 more)

### Community 4 - "Skills Repo Changesets"
Cohesion: 0.09
Nodes (32): AGENTS.md skills repo conventions, CHANGELOG mattpocock-skills, Changeset: grilling horizontal rule between questions, Changeset: grilling remove em-dashes, Changeset: remove em-dashes repo-wide, Changeset: Skill tool invocation terminology, Changeset: user-invoked skill invocation fix, Changeset: wait-what CONTEXT-MAP (+24 more)

### Community 5 - "Learning & Cognition Concepts"
Cohesion: 0.08
Nodes (29): Completion Criterion, Context load and Cognitive load, Context Pointer, Information Hierarchy, Leading Word, Lesson, Progressive Disclosure, Router Skill (+21 more)

### Community 6 - "BaseHandler"
Cohesion: 0.13
Nodes (3): BaseHandler, AppServer, withTimeout()

### Community 7 - "Tool Profiles"
Cohesion: 0.12
Nodes (23): ANALYSIS, applyProfile(), CORE_WRITE, DEFAULT_PROFILE, GUIDANCE, PROFILE_NAMES, ProfileDefinition, ProfileError (+15 more)

### Community 8 - "Env & HTTP Transport"
Cohesion: 0.14
Nodes (20): parseList(), CORS_EXPOSED_HEADERS, CORS_REQUEST_HEADERS, createRateLimiter(), extractBearerToken(), hostAllowed(), MAX_HTTP_BODY_BYTES, normalizeOrigin() (+12 more)

### Community 9 - "Wayfinder & Ticket Mapping"
Cohesion: 0.10
Nodes (23): Wayfinder decision-ticket map, docs/agents config files, Ticket task graph and frontier, Triage roles state machine, implement skill doc, improve-codebase-architecture skill doc, prototype skill doc, setup-matt-pocock-skills skill doc (+15 more)

### Community 10 - "Doc Generation Script"
Cohesion: 0.09
Nodes (15): rendered, root, size, target, child, exited, failures, responses (+7 more)

### Community 11 - "In-Memory Notes Backend"
Cohesion: 0.15
Nodes (5): createBackend(), InMemoryNotesBackend, NoteStore, setup(), tickingClock()

### Community 12 - "Skills Handlers"
Cohesion: 0.23
Nodes (15): SkillsHandlers, discoverSkills(), findSkill(), parseFrontmatter(), readSkillFile(), Skill, SKILL_URI_PREFIX, skillByUri() (+7 more)

### Community 13 - "Dev Package & Changesets Tooling"
Cohesion: 0.11
Nodes (18): @changesets/changelog-github, @changesets/cli, description, devDependencies, @changesets/changelog-github, @changesets/cli, license, name (+10 more)

### Community 14 - "Template Setup Script"
Cohesion: 0.23
Nodes (17): ask(), ask_secret(), banner(), _clear(), _existing(), finish(), note(), open_url() (+9 more)

### Community 15 - "Writing Skills"
Cohesion: 0.14
Nodes (15): Writing Fragments skill, Fragment, Leading word, Writing Fragments openai.yaml, Writing Shape skill, Grounding, Writing Shape openai.yaml, Productivity README (+7 more)

### Community 16 - "Tests & Fake Backend Helpers"
Cohesion: 0.19
Nodes (11): vitest, fakeBackend(), ACCEPTED, BASE_ENV, headers(), initializeMessage, openSession(), post() (+3 more)

### Community 17 - "Skills ADRs & Setup"
Cohesion: 0.15
Nodes (13): Hard vs soft dependency skills, setup-matt-pocock-skills, Skills ADR-0001: explicit setup pointer only for hard dependencies, Skills ADR-0002: ship as a Claude Code plugin, defer Codex plugin, skills.sh universal installer, Canonical install block, Model-invoked vs user-invoked skills, Skill dependencies via the Skill tool (+5 more)

### Community 18 - "Notes Types"
Cohesion: 0.14
Nodes (11): EXAMPLE_NOTES, InMemoryNotesOptions, NewNote, normaliseTags(), Note, NotePatch, NOTES_FEATURES, NoteSearch (+3 more)

### Community 19 - "TypeScript Config"
Cohesion: 0.14
Nodes (13): compilerOptions, esModuleInterop, forceConsistentCasingInFileNames, module, moduleResolution, outDir, rootDir, skipLibCheck (+5 more)

### Community 20 - "Changesets Config"
Cohesion: 0.15
Nodes (12): access, baseBranch, changelog, commit, fixed, ignore, linked, privatePackages (+4 more)

### Community 23 - "Git Guardrails & Shoehorn"
Cohesion: 0.18
Nodes (11): Misc README, Git Guardrails for Claude Code skill, PreToolUse git block hook, Git Guardrails for Claude Code openai.yaml, Migrate to Shoehorn skill, shoehorn fromPartial/fromAny, Migrate to Shoehorn openai.yaml, Scaffold Exercises skill (+3 more)

### Community 24 - "Backend Errors"
Cohesion: 0.29
Nodes (6): isPermanent(), PermanentBackendError, SessionExpiredError, BackendOptions, BASE_ENV, connect()

### Community 25 - "Registry server.json"
Cohesion: 0.22
Nodes (8): description, name, packages, repository, source, url, $schema, version

### Community 26 - "Handoff & Loop Skills"
Cohesion: 0.25
Nodes (8): Article beats journey, Grilling session, Claude Handoff openai.yaml, claude-handoff skill, Loop Me openai.yaml, loop-me skill, In Progress README, writing-beats skill

### Community 27 - "Fake Backend"
Cohesion: 0.32
Nodes (6): HealthReport, DOMAIN_METHODS, FakeBackendOptions, LIFECYCLE, recordingBackend(), seedStore()

### Community 28 - "Triage & Agent Briefs"
Cohesion: 0.33
Nodes (7): Agent brief, .out-of-scope knowledge base, ready-for-agent state, Writing Agent Briefs, Triage openai.yaml, Out-of-Scope Knowledge Base, triage skill

### Community 29 - "Domain Docs & TDD"
Cohesion: 0.29
Nodes (6): CONTEXT.md glossary, Domain Docs Consumer Rules, TDD openai.yaml, TDD Mocking Guidelines, TDD Skill, Good and Bad Tests

### Community 31 - "Research & Merge Skills"
Cohesion: 0.29
Nodes (7): Primary sources, research skill doc, resolving-merge-conflicts skill doc, Research openai.yaml, Research Skill, Resolving Merge Conflicts openai.yaml, Resolving Merge Conflicts Skill

### Community 32 - "Issue Tracker Setup"
Cohesion: 0.38
Nodes (7): Five canonical triage roles, Setup Skills openai.yaml, Issue Tracker GitHub, Issue Tracker GitLab, Issue Tracker Local Markdown, Setup Matt Pocock Skills, Triage Labels Mapping

### Community 34 - "Architecture Improvement"
Cohesion: 0.33
Nodes (3): Deepening opportunity, Setup TS Deep Modules openai.yaml, setup-ts-deep-modules skill

### Community 35 - "Prototype Skill"
Cohesion: 0.50
Nodes (4): Prototype openai.yaml, Prototype Logic Branch, Prototype Skill, Prototype UI Branch

### Community 36 - "HITL Loop Script"
Cohesion: 0.83
Nodes (3): capture(), hitl-loop.template.sh script, step()

### Community 37 - "Wizard Skill"
Cohesion: 0.67
Nodes (3): Interactive bash wizard, Wizard openai.yaml, wizard skill

## Knowledge Gaps
- **94 isolated node(s):** `@types/node`, `@vitest/coverage-v8`, `typescript`, `@changesets/changelog-github`, `@changesets/cli` (+89 more)
  These have ≤1 connection - possible missing edges or undocumented components. (Counts symbols only; 299 node(s) total have ≤1 connection when file, concept and rationale nodes are included.)
- **16 thin communities (<3 nodes) omitted from report** — run `graphify query` to explore isolated nodes.

## Suggested Questions
_Questions this graph is uniquely positioned to answer:_

- **Why does `@modelcontextprotocol/sdk` connect `Server Core & SDK` to `Config & Docs Handlers`, `Package Manifest`, `Env & HTTP Transport`, `Skills Handlers`, `Backend Errors`?**
  _High betweenness centrality (0.030) - this node is a cross-community bridge._
- **What connects `@types/node`, `@vitest/coverage-v8`, `typescript` to the rest of the system?**
  _94 weakly-connected nodes found - possible documentation gaps or missing edges._
- **Should `Server Core & SDK` be split into smaller, more focused modules?**
  _Cohesion score 0.06605222734254992 - nodes in this community are weakly interconnected._
- **Why does `AppServer` connect `BaseHandler` to `Server Core & SDK`, `Config & Docs Handlers`, `Tool Profiles`, `Env & HTTP Transport`, `Skills Handlers`, `Tests & Fake Backend Helpers`, `Backend Errors`?**
  _High betweenness centrality (0.019) - this node is a cross-community bridge._
- **Should `CI, Agents Guide & Conventions` be split into smaller, more focused modules?**
  _Cohesion score 0.05817028027498678 - nodes in this community are weakly interconnected._
- **Why does `InMemoryNotesBackend` connect `In-Memory Notes Backend` to `Tests & Fake Backend Helpers`, `Notes Types`, `Backend Interface`, `Backend Errors`, `Fake Backend`?**
  _High betweenness centrality (0.015) - this node is a cross-community bridge._
- **Should `Config & Docs Handlers` be split into smaller, more focused modules?**
  _Cohesion score 0.10384615384615385 - nodes in this community are weakly interconnected._