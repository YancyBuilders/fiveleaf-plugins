# FiveLeaf Themes

This plugin adds eleven themes to the built-in FiveLeaf theme. Ayu, Claude, Qoder, Grok Bot and Cursor follow the window appearance. Each has one picker entry with `path` for the light palette and `darkPath` for the dark one. The other six entries stay dark.

## Color sources

These files contain the colors used by FiveLeaf's original Go palettes, including its contrast adjustments, button states and 16 terminal colors. The FiveLeaf work is covered by the [project MIT license](LICENSE).

| Theme | Source |
| --- | --- |
| The Matrix | FiveLeaf's interpretation of the film, with steel chrome, green code, a red primary button and blue selections. |
| Claude | FiveLeaf's adaptation of Claude Code's light and dark terminal colors, including the orange accent and periwinkle selection. |
| Qoder | Qoder's Forest Light and Forest Dark workbench colors. FiveLeaf draws the syntax colors from the Forest chart series. |
| Grok Bot | Grok's Sand Light and Sand Dark palettes. The light syntax colors use the app's color primitives, and the dark syntax and ANSI colors draw on the terminal shown on x.ai. |
| Cursor | Cursor Light and Cursor Dark workbench, syntax and terminal colors, with FiveLeaf adjustments for selection visibility and contrast. |
| Purple Gold | FiveLeaf's porphyry, Tyrian purple and gold leaf palette. |
| Jack-o'-Lantern, Witch's Brew, Blood Moon | FiveLeaf's candlelit pumpkin, plum and green potion, and crimson and old gold palettes. |
| One Dark Pro | Workbench, syntax and ANSI colors from the default `themes/OneDark-Pro.json` in `zhuangtongfa.material-theme` 3.20.6, with FiveLeaf control states. [Upstream](https://github.com/Binaryify/OneDark-Pro) · [MIT license](licenses/One-Dark-Pro.txt) |
| Ayu | Light and dark palettes from `ayu-theme/ayu-colors` 9.1.0, with FiveLeaf adjustments for legibility. [Upstream revision](https://github.com/ayu-theme/ayu-colors/tree/c6e86054896ef10c69ba899dc11fdad0e004d4d3) · [MIT license](licenses/ayu-colors.txt) |

## Palette conventions

Colors encode sRGB bytes as `#rrggbb` or `#rrggbbaa`. `colors.fillHover` and `colors.fillPressed` preserve the two primary button states. One Dark Pro specifies its title bar color. The remaining themes inherit `colors.chrome` for the title bar, including when a custom theme overrides it.

All palettes use the shared workbench metrics. Qoder also specifies its card radius, grain and sentence-case headings. Additional syntax roles inherit their parent unless the palette assigns them, as One Dark Pro does for Go and JavaScript.
