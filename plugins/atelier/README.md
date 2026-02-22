# Atelier — Claude Code Plugin

AI-native animation engine with 52 MCP tools for creating, editing, previewing, and exporting declarative YAML animations.

## Install

```
/plugin marketplace add ascend42/a-atelier-plugin
/plugin install atelier@a-atelier-plugin
```

## What You Get

**52 MCP tools** across 16 groups:

| Group | Tools | Description |
|-------|-------|-------------|
| Document | 5 | Create, load, export, info, list |
| Layers | 5 | Add, edit, remove, list, reorder |
| Shapes | 3 | Set shape, fill, stroke |
| States | 4 | Add, edit, remove, list animation states |
| Deltas | 4 | Animate properties with keyframes and easing |
| Presets | 2 | Define and list reusable animation presets |
| Preview | 2 | Validate documents, preview resolved frames |
| Templates | 2 | Instantiate templates, find variables |
| Layer Effects | 5 | Blend modes, shadows, motion paths, clip paths, edit visual |
| State Config | 3 | Audio tracks, transitions, hierarchical states |
| Export | 2 | Export to SVG string or Lottie JSON |
| Assets | 3 | Manage external assets (images, fonts, audio) |
| Variables | 3 | Manage template variables |
| Interactions | 3 | Add trigger-action bindings to layers |
| Refs | 2 | Composition via ref layers |
| Performance | 4 | Profile, diff frames, batch preview, complexity analysis |

## Example Workflow

```
You: Create a loading spinner animation

Claude uses:
  atelier_create → new document (800x600, 60fps)
  atelier_add_layer → circle shape layer
  atelier_set_fill → blue solid fill
  atelier_add_state → "spin" state, 60 frames
  atelier_add_delta → rotate 0 to 360 degrees
  atelier_export → YAML output
```

## Export Formats

- **YAML** — `.atelier` declarative format
- **SVG** — static frame export
- **Lottie JSON** — web animation format
- **MP4/GIF** — via CLI (`atelier render`)

## Requirements

- Node.js >= 18
- `@a-company/atelier` npm package (installed automatically via npx)

## Links

- [Source Code](https://github.com/ascend42/a-atelier)
- [npm Package](https://www.npmjs.com/package/@a-company/atelier)
- [Format Specification](https://github.com/ascend42/a-atelier/blob/main/docs/format-spec.md)
- [MCP Tool Reference](https://github.com/ascend42/a-atelier/blob/main/docs/mcp-reference.md)
