# IntelliJ Snippets

Dart and Java snippets for the development on the K.S.C.H. Workflows project for IntelliJ and Android Studio.

## Installation

1. Download the latest release:

https://github.com/ksch-workflows/snippets/releases/latest/download/snippets.zip

2. Install Plugin from disk...

https://www.jetbrains.com/help/idea/managing-plugins.html#install_plugin_from_disk

## Dart snippets

- `uuid`: Add random UUID
- `toTest`: Add TODO comment with reminder to create a unit test
- `testWidgets`: Add minimal widget test

## Java snippets

| Keyword | Description |
|---------|-------------|
| `toTest` | Add a reminder to create a unit test |

## Development

### Add new live template

To add or edit a live template, edit it in IntelliJ, then copy it there and paste it into one of the files in [`src/main/resources/liveTemplates/`](src/main/resources/liveTemplates).

To create a new template group, create a new XML file in that directory and then copy this empty `templateSet` tag, with an custom group name:

```
<?xml version="1.0" encoding="UTF-8"?>
<templateSet group="K.S.C.H. Workflows - Dart">

</templateSet>
```

Then register the new file in the `extensions` tag of [`plugin.xml`](src/main/resources/META-INF/plugin.xml).
