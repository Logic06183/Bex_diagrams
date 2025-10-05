# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Overview

This repository contains SVG-based data visualizations documenting South African migration policy, xenophobic violence, and civil society responses from 1993-2025. All diagrams are hand-coded SVG files (not generated from data files) with embedded styling, animations, and complex visual metaphors.

## Diagram Categories

The repository includes several thematic visualization styles:

**Timeline-based diagrams:**
- Linear timelines showing policy evolution, legislative changes, and violence incidents
- Comparative timelines contrasting anti-poor vs pro-poor policies
- Phase-based timelines with swim lanes for different policy categories

**Conceptual visualizations:**
- River/stream flows representing policy convergence and divergence
- Network graphs showing causal relationships between events
- Spiral timelines showing cyclical patterns

**Thematic focus areas:**
- Migration law and legislative evolution
- Xenophobic violence incidents and patterns
- Civil society and CSO counter-mobilization
- Anti-migrant mobilization and organized movements
- Pro-poor vs anti-poor policy trajectories

## SVG Structure Patterns

All SVG files follow consistent patterns:

1. **Definitions section (`<defs>`)**: Contains reusable gradients, filters, patterns, and CSS styles
2. **Embedded CSS**: Typography classes, color schemes, and structural styling defined inline
3. **Semantic class names**: `.main-title`, `.event-label`, `.year-label`, `.phase-title`, etc.
4. **Color coding**: Consistent color palettes across files (e.g., red for violence, green for pro-poor policies, blue for migration law)
5. **Responsive viewBox**: Most diagrams use A4 landscape (842×595) or custom dimensions with proper viewBox scaling

## Common Editing Tasks

**Modifying diagram content:**
- Text elements use absolute positioning (x, y coordinates)
- Events are typically grouped in `<g>` tags with transforms
- Update both visual elements and their corresponding text labels

**Adjusting visual styling:**
- CSS classes are defined in the `<defs><style>` section
- Color schemes use named classes (`.anti-poor-box`, `.pro-poor-box`, etc.)
- Gradients and filters are referenced by ID

**Adding new events/data points:**
- Follow existing spacing and positioning patterns
- Maintain consistent class usage for styling
- Update timeline scales proportionally when adding events

## Design Conventions

- **Typography**: Arial/Helvetica sans-serif throughout, varying sizes (7px-24px) for hierarchy
- **Violence/conflict**: Red color palette (#C1292E, #DC143C, #8B0000)
- **Civil society/positive**: Green palette (#4d804d, #a8d5a8)
- **Migration law**: Blue palette (#1e3a8a, #3b82f6)
- **Scientific variants**: Files with "_scientific" suffix use subdued colors and formal styling for academic publications
- **A4 format**: Several diagrams specify A4 landscape (842×595 pixels at 72 DPI) for print compatibility

## File Naming Patterns

- Descriptive names indicating content and sometimes format (e.g., `_scientific`, `_timeline`, `_phases`)
- No build process or generated files—all SVGs are source files
