# Material Icon Theme

The Material Icon Theme provides lots of icons based on Material Design for Visual Studio Code.



## File icons

![fileIcons](img/fileIcons.png)



## Folder icons

![folderIcons](img/folderIcons.png)



## Customize folder color

You can change the color of the default folder icon using the command palette:

![set folder color](img/set-folder-color.gif)

or via user settings:

```
"material-icon-theme.folders.color": "#ef5350",
```



## Folder themes

You can change the design of the folder icons using the command palette:

![set folder theme](img/set-folder-theme.gif)

or via user settings:

```
"material-icon-theme.folders.theme": "specific"
```



## Custom icon associations

Youcan customize the icon associations directly in the user settings.



## File associations

With the `*.[extension]` pattern you can define custom file icon associations. For example you could define an icon for `*.sample` and every file that ends with `.sample` will have the defined icon. If there's no leading `*` it will be automatically configured as filename and not as file extension.

```
"material-icon-theme.files.associations": {
    "*.ts" "typescript",
    "fileName.ts": "angular"
}
```



## Folder associations

The following configuration can customize the folder icons. It is also possible to overwrite existing associations and create nice combinations. For example you could change the folder theme to "classic" and define icons only for the folder names you like.

```
"material-icon-theme.folders.associations": {
    "customFolderName": "src",
    "sample": "dist"
}
```



## Language associations

With the following configuration you can customize the language icons. It is also possible to overwrite existing associations.

```
"material-icon-theme.languages.associations": {
    "languageId": "iconName",
    "json": "json"
}
```

Available language ids:

https://code.visualstudio.com/docs/languages/identifiers#_known-language-identifiers

You can see the available icon names in the overview above.



## One-click activation

After installation or update you can click on the 'Activate'-button to activate the icon theme, if you haven't already.
The icons will be visible immediately.

![one click activation](img/oneclickactivation.png)



## Commands

Press `Ctrl-Shift-P` to open the command palette and type `Material Icons`.

![command Palette](img/commandPalette.png)

- **Change Folder Theme:** Change the design of the folder icons.
- **Restore Default Configuration:** Reset the default configurations of the icon theme.
- **Change Folder Color:** Change the color of the folder icons.
- **Hide Folder Arrows** Hides the arrows next to the folder icons.
- **Configure Icon Packs:** Select an icon pack that enables additional icons (e.g. for Angular, React, Ngrx).
- **Activate Icon Theme:** Activate the icon theme.



## Icon source

- [Material Design Icons](https://materialdesignicons.com/)
- official icons



## How to contribute

Read the [contribution guidelines](https://github.com/PKief/vscode-material-icon-theme/blob/master/CONTRIBUTING.md).

If you have some questions or icon requests open a [new issue](https://github.com/PKief/vscode-material-icon-theme/issues) on Github.



## Follow me

- [Twitter](https://twitter.com/PhilippKief)
- [Github](https://github.com/PKief)





