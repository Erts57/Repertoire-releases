# Changelog

All notable changes to Repertoire are documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

## [1.1.0] - 2026-10-22

### Added

- Inspector 2.0: tabbed object workspace (Properties, Relationships, Comments, Media, AI) with breadcrumb header, multi-select bulk edit, and field groups
- Object comments (threaded markdown, mentions, resolve)
- Project-scoped enum types and Enum fields
- Prefill enum options when creating an enum type in the inspector
- Relationship type source/target datatype restrictions (set on create or later in the inspector)
- Datatype field schema editing in the inspector (create and edit); removed from table view
- Table hierarchy mode: optional parenting via a parent relationship type (nested rows, expand/collapse, drag reparent)
- Dockable workspace layout (dockview) persisted in project settings
- Marketing website (`npm run website:dev` / `website:build`)
- Privacy Policy and Terms of Service pages; NSIS installer shows Terms; Settings → Legal links
- Custom NSIS installer icon (app mark with download badge)

### Changed

- Tree view merged into Table; separate Tree view type removed. Existing `type = "tree"` view rows are ignored (no auto-conversion)
- AI review queue moved from the sidebar into the Inspector AI tab
- Rich Text (TipTap) replaced by Markdown; legacy TipTap JSON is flattened to plain text on open
- Docs aligned with the shipping product (roadmap archive removed)

### Removed

- Inspector History tab and `object_history` / related triggers
- Favorites and Recent sidebar features
- Built-in Kanban view (custom views remain available via plugins)
- Workspace layout presets
- TipTap dependencies and example plugin packages under `examples/`

## [1.0.0] - 2026-08-05

First public release.

### Added

- Tauri 2 desktop shell with React, TypeScript, and Zustand
- SQLite persistence for projects, datatypes, objects, and properties
- Field types: text, number, boolean, date, tags, rich text, image, video, audio, time, list, and formula
- Table view with inline editing, sorting, and column visibility
- Cards, gallery, tree, timeline, and canvas views with view-specific configuration and filters
- Relationship types and first-class relationships between objects
- Full-text search (SQLite FTS5) and command palette
- Official templates and “new project from template” flow
- Light and dark themes with per-project preference
- Full project export/import (JSON bundle + media, folder or zip)
- CSV and JSON Lines interchange per datatype
- Plugin runtime with manifest, load/unload, and plugin manager UI
- Registration APIs for views, commands, field types, importers, exporters, themes, and widgets
- Optional AI assistance with pluggable providers (OpenAI, Anthropic, Ollama, embedded llama.cpp)
- Schema-aware prompts, selection-aware AI actions, and review-before-apply flows
- Cross-platform release pipeline (Windows, macOS) publishing to a public releases repository
- Auto-update via Tauri updater plugin and signed update artifacts
- Bundle format migration framework and documented upgrade path
- Explicit SQLite `user_version` schema tracking
- Changelog-driven GitHub Release notes
- Maintainer docs for releases and deferred OS code signing

### Changed

- App version is sourced from `package.json` (single source of truth)

[Unreleased]: https://github.com/Erts57/Repertoire-releases/releases/latest
[1.1.0]: https://github.com/Erts57/Repertoire-releases/releases/tag/v1.1.0
[1.0.0]: https://github.com/Erts57/Repertoire-releases/releases/tag/v1.0.0
