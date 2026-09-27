# Changelog

## [3.0.0] - 2026-09-27

### Changed
- **BREAKING:** the skill is named `bug-fix-lifecycle`, like its folder, its repository and its Claude Code agent. It was `defect-lifecycle-agent-skill`; the trigger is now `$bug-fix-lifecycle`. `package.json`, `agents/openai.yaml`, the README and the schema `$id`s follow.
- `disable-model-invocation: true`: the chain runs as a Claude Code agent (`bug-fix-lifecycle`) instead of being picked from its description.
- New "Chain Phases" section, generated from `config/chain_definition.json`: engine phase, skill, gate, and the matching step of this SKILL.md's workflow. `config/chain_definition.json` is now committed.
- `package.json` version realigned (it still said 2.2.0).

## [2.2.1] - 2026-04-30

### Changed
- Trim `SKILL.md` frontmatter to fit the 1000-character dispatcher limit (description trim, migrate non-dispatcher fields to body).

## 2.2.0 - 2026-04-19

- aligned the skill frontmatter and trigger with the canonical `defect-lifecycle-agent-skill` identity
- synced public docs, schema identifiers, and validation metadata with the canonical repository
- confirmed `jovd83/defect-lifecycle-agent-skill` as the active source of truth before retiring the legacy private repo

## 2.1.0 - 2026-03-21

- polished the public-facing repo and package identity to `defect-lifecycle-agent-skill`
- added canonical JSON schemas and example artifacts for discovery and fix reports
- added Jira-ready and Linear-ready tracker draft exports with a dedicated CLI script
- expanded validation coverage to include schema fixtures and tracker export behavior

## 2.0.0 - 2026-03-21

- rewrote the core skill contract around repository-aware bug reporting and approved-fix execution
- replaced brittle, emoji-heavy templates with stronger traceable report formats
- upgraded the coverage helper to support thresholds, metrics, manifests, and file-scoped validation
- added references, examples, validation scripts, tests, install metadata, and GitHub workflow packaging
