# FiveLeaf plugins

Browse each color theme and file icon set below. Click a name to open its files and installation instructions. In FiveLeaf, search **Settings → Plugins** for the same name.

## Color themes

| Plugin | Preview | Install |
| --- | --- | --- |
| [One Dark Pro](one-dark-pro/) | <img src="one-dark-pro/preview.svg" alt="One Dark Pro preview" height="68"> | `fiveleaf plugin install one-dark-pro` |
| [Ayu](ayu/) | <img src="ayu/preview.svg" alt="Ayu preview" height="68"> | `fiveleaf plugin install ayu` |
| [Blood Moon](blood-moon/) | <img src="blood-moon/preview.svg" alt="Blood Moon preview" height="68"> | `fiveleaf plugin install blood-moon` |
| [Claude](claude/) | <img src="claude/preview.svg" alt="Claude preview" height="68"> | `fiveleaf plugin install claude` |
| [Cursor](cursor/) | <img src="cursor/preview.svg" alt="Cursor preview" height="68"> | `fiveleaf plugin install cursor` |
| [Grok Bot](grok-bot/) | <img src="grok-bot/preview.svg" alt="Grok Bot preview" height="68"> | `fiveleaf plugin install grok-bot` |
| [Jack-o'-Lantern](jack-o-lantern/) | <img src="jack-o-lantern/preview.svg" alt="Jack-o&#x27;-Lantern preview" height="68"> | `fiveleaf plugin install jack-o-lantern` |
| [Purple Gold](purple-gold/) | <img src="purple-gold/preview.svg" alt="Purple Gold preview" height="68"> | `fiveleaf plugin install purple-gold` |
| [Qoder](qoder/) | <img src="qoder/preview.svg" alt="Qoder preview" height="68"> | `fiveleaf plugin install qoder` |
| [The Matrix](the-matrix/) | <img src="the-matrix/preview.svg" alt="The Matrix preview" height="68"> | `fiveleaf plugin install the-matrix` |
| [Witch's Brew](witchs-brew/) | <img src="witchs-brew/preview.svg" alt="Witch&#x27;s Brew preview" height="68"> | `fiveleaf plugin install witchs-brew` |

## File icon themes

| Plugin | Preview | Install |
| --- | --- | --- |
| [Material Icon Theme](material-icons/) | <img src="material-icons/preview.svg" alt="Material Icon Theme preview" height="42"> | `fiveleaf plugin install material-icons` |
| [Ayu Icons](ayu-icons/) | <img src="ayu-icons/preview.svg" alt="Ayu Icons preview" height="42"> | `fiveleaf plugin install ayu-icons` |
| [Catppuccin Latte Icons](catppuccin-latte-icons/) | <img src="catppuccin-latte-icons/preview.svg" alt="Catppuccin Latte Icons preview" height="42"> | `fiveleaf plugin install catppuccin-latte-icons` |
| [Catppuccin Mocha Icons](catppuccin-mocha-icons/) | <img src="catppuccin-mocha-icons/preview.svg" alt="Catppuccin Mocha Icons preview" height="42"> | `fiveleaf plugin install catppuccin-mocha-icons` |
| [FiveLeaf File Icons](fiveleaf-file-icons/) | <img src="fiveleaf-file-icons/preview.svg" alt="FiveLeaf File Icons preview" height="42"> | `fiveleaf plugin install fiveleaf-file-icons` |
| [Seti Icons](seti-icons/) | <img src="seti-icons/preview.svg" alt="Seti Icons preview" height="42"> | `fiveleaf plugin install seti-icons` |

The built-in FiveLeaf color theme is available on first launch. Each adaptive theme includes its light and dark palettes in one plugin. Color themes and file icons can be mixed freely.

## Switching from the original bundles

Install the individual themes and icon sets you use. Then remove the old bundles with `fiveleaf plugin remove fiveleaf-themes` and `fiveleaf plugin remove fiveleaf-icons`. FiveLeaf recognizes your saved selections.

## Local development

Run `fiveleaf plugin dev ./one-dark-pro` from this checkout to work on One Dark Pro. Each plugin directory contains a manifest, its own assets, a preview and its licenses. The marketplace reads [index.json](index.json).
