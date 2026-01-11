---
name: mermaid-visualizer
description: Transform text content into professional Mermaid diagrams for presentations and documentation. Use when users ask to visualize concepts, create flowcharts, or make diagrams from text. Supports process flows, system architectures, comparisons, mindmaps, and more with built-in syntax error prevention.
metadata:
  version: 1.1.0
---

# Mermaid Visualizer

Convert text content into clean, professional Mermaid diagrams optimized for presentations and documentation.

## Quick Start

1. **Analyze content** - Identify key concepts, relationships, and flow
2. **Choose diagram type** - Select the most appropriate visualization
3. **Select configuration** - Determine layout, detail level, and styling
4. **Generate diagram** - Create syntactically correct Mermaid code
5. **Output in markdown** - Wrap in proper code fence

**Defaults:** Vertical layout (TB), medium detail, professional colors, Obsidian/GitHub compatible.

## Diagram Types

| Type | Best For |
|------|----------|
| **Process Flow** (graph TB/LR) | Workflows, decision trees, AI agent architectures |
| **Circular Flow** | Cyclic processes, feedback loops |
| **Comparison** | Before/after, A vs B analysis |
| **Mindmap** | Hierarchical concepts, knowledge organization |
| **Sequence Diagram** | Component interactions, API calls |
| **State Diagram** | System states, status transitions |

## Critical Syntax Rules

**Rule 1: Avoid List Syntax Conflicts**
```
❌ [1. Perception]    → Triggers parsing error
✅ [1.Perception]     → Remove space after period
✅ [① Perception]     → Use circled numbers
```

**Rule 2: Subgraph Naming**
```
❌ subgraph AI Agent Core    → Space without quotes
✅ subgraph agent["AI Agent Core"]  → Use ID with display name
```

**Rule 3: Node References**
```
❌ Title --> AI Agent Core   → Reference display name
✅ Title --> agent           → Reference subgraph ID
```

**Rule 4: Special Characters**
- Quotation marks → use 『』
- Parentheses → use 「」

**Rule 5: Arrow Types**
- `-->` solid, `-.->` dashed, `==>` thick, `~~~` invisible

## Configuration Options

**Layout:** TB (vertical), LR (horizontal), RL, BT
**Detail:** simple, standard, detailed, presentation
**Style:** minimal, professional, colorful, academic
**Extras:** show_legend, numbered, title

## Color Palette

- Green (#d3f9d8): Input, start states
- Red (#ffe3e3): Planning, decisions
- Purple (#e5dbff): Processing, reasoning
- Orange (#ffe8cc): Actions, tools
- Cyan (#c5f6fa): Output, results
- Yellow (#fff4e6): Storage, memory

## Quality Checklist

- [ ] No "number. space" patterns in node text
- [ ] All subgraphs use ID["display name"] format
- [ ] Arrow syntax correct
- [ ] Colors applied consistently
- [ ] Compatible with Obsidian/GitHub

## References

For complete syntax rules and troubleshooting: [references/syntax-rules.md](references/syntax-rules.md)
