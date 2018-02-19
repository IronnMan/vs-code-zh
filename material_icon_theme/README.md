# Material Icon Theme

Material Icon Theme 提供了许多基于 Visual Studio Code 的 [Material Design](http://www.uisdc.com/comprehensive-material-design-note)。



## File icons

![fileIcons](img/fileIcons.png)



## Folder icons

![folderIcons](img/folderIcons.png)



## Customize folder color

您可以使用命令面板更改默认文件夹图标的颜色：

![set folder color](img/set-folder-color.gif)

或通过用户设置：

```
"material-icon-theme.folders.color": "#ef5350",
```



## Folder themes

您可以使用命令面板更改文件夹图标的设计：

![set folder theme](img/set-folder-theme.gif)

或通过用户设置：

```
"material-icon-theme.folders.theme": "specific"
```



## Custom icon associations

你可以直接在用户设置中自定义图标关联。



### File associations

使用 `*.[extension]` 模式，您可以定义自定义文件图标关联。例如，您可以为 `*.sample` 文件定义一个图标，并且每个以 `.sample` 结尾的文件都将具有定义的图标。如果没有前导 `*` ，它将自动配置为文件名而不是文件扩展名。

```
"material-icon-theme.files.associations": {
    "*.ts" "typescript",
    "fileName.ts": "angular"
}
```



### Folder associations

以下配置可以自定义文件夹图标。也可以覆盖现有的关联并创造出色的组合。例如，您可以将文件夹主题更改为 "classic"，并仅为您喜欢的文件夹名称定义图标。

```
"material-icon-theme.folders.associations": {
    "customFolderName": "src",
    "sample": "dist"
}
```



### Language associations

通过以下配置，您可以自定义语言图标。也可以覆盖现有的关联。

```
"material-icon-theme.languages.associations": {
    "languageId": "iconName",
    "json": "json"
}
```

可用语言 ID：

https://code.visualstudio.com/docs/languages/identifiers#_known-language-identifiers

您可以在上面的概述中看到可用的图标名称。



## One-click activation

安装后，如果您还没有更新，您可用点击 'Activate' 按钮激活图标主题。
图标将立即可见。

![one click activation](img/oneclickactivation.png)



## Commands

按下 `Ctrl-Shift-P` 打开命令选项版并输入 `Material Icons`。

![command Palette](img/commandPalette.png)

- **Change Folder Theme:** 更改文件夹图标的设计。
- **Restore Default Configuration:** 重置图标主题的默认配置。
- **Change Folder Color:** 更改文件夹图标的颜色。
- **Hide Folder Arrows:** 隐藏文件夹图标旁边的箭头。
- **Configure Icon Packs:** 选择一个启用其他图标的图标包（例如，用于 Angular, React, Ngrx）
- **Activate Icon Theme:** 激活图标主题。



## Icon source

- [Material Design Icons](https://materialdesignicons.com/)
- official icons



## 如何贡献

阅读[贡献指南](https://github.com/PKief/vscode-material-icon-theme/blob/master/CONTRIBUTING.md)。

如果您有任何问题或图标请求，请在 Github 上打开一个[新问题](https://github.com/PKief/vscode-material-icon-theme/issues)。



## Follow me

- [Twitter](https://twitter.com/PhilippKief)
- [Github](https://github.com/PKief)





