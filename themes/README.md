# Themes

PlantUML supports defining themes which can be used to control color, font, and other values consistently.  This folder is intended to contain CarGurus specific PlantUML theme files.

## Using theme files

To use a theme file, within your plantUML diagram you should use an `!theme` directive and specify the [raw location](https://docs.github.com/en/enterprise-cloud@latest/repositories/working-with-files/using-files/viewing-a-file#viewing-or-copying-the-raw-file-content) of the `themes` folder in this repo.  For more details see the PlantUML docs on using [Themes from the Internet](https://plantuml.com/theme#f701ab9af850cc25).

### Example
```text
!theme CarGurus-C4-default from https://raw.githubusercontent.com/cargurus/plantuml-common/main/themes
```

## Creating theme files

For how to author theme files, review the C4-PlantUML [Themes README file](https://github.com/kirchsth/C4-PlantUML/blob/extended/Themes.md).

Themes are useful but [style files](/styles/README.md) can fulfill most purposes that themes do and are simpler to author because you can use higher level macros to express your choices.

### Naming theme files

CarGurus theme files should be named `puml-theme-CarGurus-[your-exact-theme-name].puml`.  Additionally, the theme name within the file must exactly match the `CarGurus-[your-exact-theme-name]` portion of the file name.  So the first line of your theme file should be:

```text
!$THEME = "CarGurus-[your-exact-theme-name]"
```
