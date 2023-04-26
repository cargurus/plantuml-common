# Styles

Similar to themes, styles are files that can be includes in new PlantUML files to provide a baseline of color, font, and other choices.  And advantage of style files over themes is that style files leverage higher abstraction macros to achieve this.  This makes them easier to author but offers less fine-grained control in some cases.

## Using style files

To use a style file, within your plantUML diagram you should use an `!include` directive and specify the [raw location](https://docs.github.com/en/enterprise-cloud@latest/repositories/working-with-files/using-files/viewing-a-file#viewing-or-copying-the-raw-file-content) of the style file in this repo.

### Example
```text
!include https://raw.githubusercontent.com/cargurus/plantuml-common/main/styles/style-CarGurus-C4-default.puml
```

## Creating style files

To create a new style, create a file in this folder and specify the desired tags or styles macro calls within it.

For a list of tags and style macros, as well as examples of use, review the C4-PlantUML [Styles section](https://github.com/kirchsth/C4-PlantUML#custom-tagsstereotypes-support-and-skinparam-updates) of their README.

### Naming style files

CarGurus style files should be named `puml-style-CarGurus-[your-style-name].puml`.