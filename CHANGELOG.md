# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [1.1.0] - 2025-01-12

### Added
- `marketplace.json` for one-command plugin installation
- Unified version numbers across all skills
- CHANGELOG.md for tracking changes

### Changed
- Optimized `mermaid-visualizer/SKILL.md` to be under 1000 words
- Moved detailed Mermaid documentation to `references/syntax-rules.md`
- Standardized metadata format in all SKILL.md frontmatter

### Fixed
- Consistent version format across all skill files

## [1.0.0] - 2025-01-11

### Added
- Initial release of Obsidian Visual Skills Pack
- **excalidraw-diagram**: Generate hand-drawn style Excalidraw diagrams
  - 8 diagram types: Flowchart, Mind Map, Hierarchy, Relationship, Comparison, Timeline, Matrix, Freeform
  - Full Chinese text support
  - Auto-save to Obsidian-ready `.md` files
- **mermaid-visualizer**: Transform text into Mermaid diagrams
  - 6 diagram types: Process Flow, Circular Flow, Comparison, Mindmap, Sequence, State
  - Built-in syntax error prevention
  - Configurable layouts and styles
- **obsidian-canvas-creator**: Create Obsidian Canvas files
  - MindMap and Freeform layouts
  - Smart node sizing and positioning
  - Color-coded nodes with 6 presets
- Comprehensive documentation in English and Chinese
- MIT License

[1.1.0]: https://github.com/eugenechen0514/axton-obsidian-visual-skills/compare/v1.0.0...v1.1.0
[1.0.0]: https://github.com/eugenechen0514/axton-obsidian-visual-skills/releases/tag/v1.0.0
