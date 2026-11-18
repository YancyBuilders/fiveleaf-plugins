# Material Icon Theme

Material Icon Theme artwork for files and folders in FiveLeaf.

![Material Icon Theme preview](preview.svg)

```sh
fiveleaf plugin install material-icons
```

Open **File Icon Theme…** in the command palette and choose **Material Icon Theme**.

Material file SVGs and closed named folder SVGs are unchanged. Its default file/folder icons and expanded folder variants are generated from the exact upstream paths in `src/core/generator/{fileGenerator,folderGenerator}.ts` and `src/scripts/svg/generateOpenFolderIcons.ts`. The default icons use the upstream default `#90a4ae` from `src/core/generator/config/defaultConfig.ts`; named folders keep their upstream colors and motifs.

Sources for individual icons are recorded in [sources.json](assets/sources.json). [Upstream snapshot](https://github.com/material-extensions/vscode-material-icon-theme/tree/ced21b9b5241c1efa502a8c46ec7363a690a7058) · [Artwork license](assets/LICENSE)
