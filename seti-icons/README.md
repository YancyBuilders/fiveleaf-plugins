# Seti Icons

Seti artwork for files and folders in FiveLeaf.

![Seti Icons preview](preview.svg)

```sh
fiveleaf plugin install seti-icons
```

Open **File Icon Theme…** in the command palette and choose **Seti**.

Seti retains the original SVG geometry and applies the colors that its Atom icon font receives from `styles/components/icons/mapping.less` and `styles/ui-variables.less`. Each glyph is painted in its mapped upstream color, including inherited fills. The default file uses `@white`, folders and configuration files use `@grey-light`, and the Git directory uses `@ignore`. Go uses the upstream `go2` file glyph. Seti has no expanded folder or dedicated source/dependency-folder SVGs, so those folders retain its standard folder icon. Seti's glyph source canvases include substantial font whitespace (for example React uses about 20×18 units of a 32×32 canvas, while the default file uses about 412×446 of 1200×1000). The upstream UI draws its icon font at 22px. For the app's 16–18px SVG slots, every Seti `viewBox` is centered on its painted bounds in a square with 6.25% margin on each side of the longest dimension. Bounds were measured with FiveLeaf's SVG renderer at 1024px; only the `viewBox` changes, so all path geometry, aspect ratios and colors remain intact. Naturally wide wordmarks stay wide.

Sources for individual icons are recorded in [sources.json](assets/sources.json). [Upstream snapshot](https://github.com/jesseweed/seti-ui/tree/2d6c5e68b4ded73c92dac291845ee44e1182d511) · [Artwork license](assets/LICENSE)
