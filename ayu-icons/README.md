# Ayu Icons

Ayu artwork for files and folders in FiveLeaf.

![Ayu Icons preview](preview.svg)

```sh
fiveleaf plugin install ayu-icons
```

Open **File Icon Theme…** in the command palette and choose **Ayu**.

Ayu uses the default file and folder artwork from its official VS Code icon theme. Its SVG files are copied unchanged, including their colors and geometry. Ten upstream assets are 32×32 PNGs; each is represented by SVG paths covering horizontal runs of identical RGBA pixels, preserving the original pixels and transparency for FiveLeaf's SVG loader. `sources.json` identifies those conversions. The FiveLeaf host keeps the original PNGs in `cmd/fiveleaf/testdata/ayu-icons` for renderer comparisons. The pack uses Ayu's default/dark assets in every appearance, its standard collapsed and expanded folder icons apply to all folders. No custom named-folder artwork is added. Ayu is distributed under its original MIT license, Copyright (c) 2016 Ike Kurghinyan.

Sources for individual icons are recorded in [sources.json](assets/sources.json). [Upstream snapshot](https://github.com/ayu-theme/vscode-ayu/tree/605c9c8504682854d77adc0b630742182a86676b) · [Artwork license](assets/LICENSE)
