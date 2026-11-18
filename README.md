# FiveLeaf plugins

The official color themes and file icons for FiveLeaf. Install them independently in **Settings → Plugins** or from the command line.

```sh
fiveleaf plugin install fiveleaf-themes
fiveleaf plugin install fiveleaf-icons
```

| Plugin | Included choices |
| --- | --- |
| [FiveLeaf Themes](fiveleaf-themes/) | One Dark Pro, Ayu, The Matrix, Claude, Qoder, Grok Bot, Cursor, Purple Gold, Jack-o'-Lantern, Witch's Brew and Blood Moon |
| [FiveLeaf Icons](fiveleaf-icons/) | FiveLeaf, Catppuccin Latte, Catppuccin Mocha, Material, Seti and Ayu |

Choose a color theme or file icon theme under **Settings → Appearance**. FiveLeaf remembers each selection when its plugin is disabled or removed.

## Local development

From this checkout, link either plugin into FiveLeaf and edit its JSON or SVG files to preview changes.

```sh
fiveleaf plugin dev ./fiveleaf-themes
fiveleaf plugin dev ./fiveleaf-icons
```

The marketplace reads [index.json](index.json). Each entry points to a plugin directory in this Git repository. The plugin directories include their licenses and upstream artwork credits.
