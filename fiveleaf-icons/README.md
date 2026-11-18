# FiveLeaf File Icons

Install this plugin to use FiveLeaf's original language-colored symbols, Catppuccin Latte and Mocha,
Material Icon Theme, Seti, or Ayu. Choose a pack in **Settings → Appearance → File Icons**, or use
**File Icon Theme…** to preview it in one window before saving the selection.

```sh
fiveleaf plugin install 'https://github.com/YancyBuilders/fiveleaf-plugins.git#fiveleaf-icons'
```

For local development, run `fiveleaf plugin dev .` from this folder. The plugin consists of its manifest,
JSON selectors, SVGs, and licenses. All paths resolve inside the plugin directory.

| Icon theme | `iconTheme` setting |
| --- | --- |
| FiveLeaf | `fiveleaf-icons.fiveleaf` |
| Catppuccin Latte | `fiveleaf-icons.catppuccin-latte` |
| Catppuccin Mocha | `fiveleaf-icons.catppuccin-mocha` |
| Material Icon Theme | `fiveleaf-icons.material` |
| Seti | `fiveleaf-icons.seti` |
| Ayu | `fiveleaf-icons.ayu` |

An empty `iconTheme` selects FiveLeaf. Its original short setting values also work. An unavailable choice
uses the installed FiveLeaf default, or generic file and folder symbols when that default is unavailable.
The saved choice takes effect again when its plugin is enabled.

## FiveLeaf selectors and colors

The original FiveLeaf shapes in `themes/fiveleaf/icons` use Lucide artwork. The `theme.json` in that folder
associates each filename with a shape and a tint. Other plugins can use the same optional fields.

- `fileNames` wins on an exact basename. Next, the longest matching `fileNamePrefixes` key wins. For example,
  `.env` matches both `.envrc` and `.env.development.json`.
- `dotfile` selects an icon for names with one leading dot and no further dots, including `.gitignore`.
  Remaining names use the longest matching `fileExtensions` suffix, then `file`. All matches ignore case.
- `tints` maps local icon IDs to a palette role such as `{"role":"accent"}`, or to language colors such as
  `{"dark":"#00add8","light":"#00809f"}`. A role follows the active palette. A language tint follows its
  light or dark appearance. Monochrome palettes mix their muted and accent colors using the dark tint's luminance.
- Icons with a tint render as a single-color glyph. Other icons keep their SVG colors in every palette,
  with `currentColor` resolved against the window's text color. Several icon IDs can use the same SVG with different tints.

## Artwork and licenses

The FiveLeaf selectors are covered by the plugin's MIT license. The Lucide artwork and its notices are in
`themes/fiveleaf/`. Each third-party pack has its original MIT `LICENSE`, `theme.json` associations and
`sources.json` mapping each local icon to its upstream source.
The named snapshots are the Git commit ids recorded in the downloaded GitHub source archives.

| Pack | Upstream | Commit |
| --- | --- | --- |
| Catppuccin Latte, Mocha | https://github.com/catppuccin/zed-icons | `f695ec0d81d53d6776471c3d3cad702cf11670e3` |
| Material | https://github.com/material-extensions/vscode-material-icon-theme | `ced21b9b5241c1efa502a8c46ec7363a690a7058` |
| Seti | https://github.com/jesseweed/seti-ui | `2d6c5e68b4ded73c92dac291845ee44e1182d511` |
| Ayu 1.6.0 | https://github.com/ayu-theme/vscode-ayu | `605c9c8504682854d77adc0b630742182a86676b` |

## Adaptations

- Catppuccin SVG geometry and colors are copied unchanged from `icons/{latte,mocha}`. Local filenames
  use shared semantic names; both flavors retain their upstream palettes.
- Material file SVGs and closed named folder SVGs are unchanged. Its default file/folder icons and expanded folder
  variants are generated from the exact upstream paths in `src/core/generator/{fileGenerator,folderGenerator}.ts`
  and `src/scripts/svg/generateOpenFolderIcons.ts`. The default icons use the upstream default `#90a4ae` from
  `src/core/generator/config/defaultConfig.ts`; named folders keep their upstream colors and motifs.
- Seti retains the original SVG geometry and applies the colors that its Atom icon font receives from
  `styles/components/icons/mapping.less` and `styles/ui-variables.less`. Each glyph is painted in its mapped upstream
  color, including inherited fills. The default file uses `@white`, folders and configuration files use
  `@grey-light`, and the Git directory uses `@ignore`. Go uses the upstream `go2` file glyph. Seti has no expanded
  folder or dedicated source/dependency-folder SVGs, so those folders retain its standard folder icon.
  Seti's glyph source canvases include substantial font whitespace (for example React uses about 20×18 units of a
  32×32 canvas, while the default file uses about 412×446 of 1200×1000). The upstream UI draws its icon font at 22px.
  For the app's 16–18px SVG slots, every Seti `viewBox` is centered on its painted bounds in a square with 6.25% margin
  on each side of the longest dimension. Bounds were measured with FiveLeaf's SVG renderer at 1024px; only the
  `viewBox` changes, so all path geometry, aspect ratios and colors remain intact. Naturally wide wordmarks stay wide.
- Associations are a curated common-language subset for FiveLeaf. Multiple extensions can share an upstream icon;
  React TSX, Go module files and TOML reuse the closest available Seti glyph. No rasterization or path simplification
  is applied. SVG XML serialization is normalized only for generated Material folders and Seti color application.
- Ayu uses the default file and folder artwork from its official VS Code icon theme. Its SVG files are copied
  unchanged, including their colors and geometry. Ten upstream assets are 32×32 PNGs; each is represented by SVG
  paths covering horizontal runs of identical RGBA pixels, preserving the original pixels and transparency for
  FiveLeaf's SVG loader. `sources.json` identifies those conversions. The FiveLeaf host keeps the original PNGs
  in `cmd/fiveleaf/testdata/ayu-icons` for renderer comparisons. The pack uses Ayu's default/dark assets in every appearance,
  its standard collapsed and expanded folder icons apply to all folders. No custom named-folder artwork is added.
  Ayu is distributed under its original MIT license, Copyright (c) 2016 Ike Kurghinyan.

## Included assets

| Pack | SVG files | Bytes, including manifest, provenance and license |
| --- | ---: | ---: |
| `catppuccin-latte` | 58 | 40,538 |
| `catppuccin-mocha` | 58 | 40,538 |
| `material` | 58 | 44,522 |
| `seti` | 44 | 43,661 |
| `ayu` | 66 | 183,530 |

The FiveLeaf pack adds 10 SVG shapes, shared by 24 icon IDs.
