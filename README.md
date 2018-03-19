# Markdown Support for Visual Studio Code

> Custom fork of the Markdown All-in-one extension
>
> [Download the extension here.](https://github.com/Radcho/vscode-markdown/raw/master/markdown-all-in-one-1.1.0.vsix)

All you need for Markdown (keyboard shortcuts, table of contents, auto preview and more).

## Features

- **Keyboard shortcuts** (toggle bold, italic, code span, strikethrough and heading)
  - Tip: in normal mode, `**word|**` -> `**word**|` (<kbd>ctrl</kbd> + <kbd>b</kbd>)
  - *Quick styling mode*: toggle bold/italic without selecting words
- **Table of contents** (No additional annoying tags like `<!-- TOC -->`)
- **Outline view** in explorer panel
- **Automatically show preview** when opening a Markdown file (Disabled by default)
- **Print Markdown to HTML**
  - It's recommended to print the exported HTML to PDF with browser (e.g. Chrome) if you want to share your documents with others
- **List editing** (when pressing <kbd>Enter</kbd> at the end of a list item) (also work for quote block)
  - Pressing <kbd>Tab</kbd> at the beginning of a list item will indent it
  - Pressing <kbd>Backspace</kbd> at the beginning of a list item will unindent it (or delete the list marker)
  - Blank list item won't be continued
- **GitHub Flavored Markdown**
  - Table formatter
  - Task lists
- **Word completion** (moved to a standalone extension [Dictionary Completion](https://marketplace.visualstudio.com/items?itemName=yzhang.dictionary-completion))

### Keyboard Shortcuts

![shortcuts1](images/gifs/bold-normal.gif)

![shortcuts2](images/gifs/bold-quick.gif)

![shortcuts3](images/gifs/heading.gif)

### Table of Contents

![toc](images/gifs/toc.gif)

### List Editing

![list editing](images/gifs/list-editing.gif)

### Table Formatter

![table formatter](images/gifs/table-formatter.gif)

### Outline

![outline](images/outline.png)

### Task Lists

![task lists](images/gifs/tasklists.gif)

## Shortcuts

| Key                                               | Command                      |
| ------------------------------------------------- | ---------------------------- |
| <kbd>ctrl</kbd> + <kbd>b</kbd>                    | Toggle bold                  |
| <kbd>ctrl</kbd> + <kbd>i</kbd>                    | Toggle italic                |
| <kbd>ctrl</kbd> + <kbd>shift</kbd> + <kbd>]</kbd> | Toggle heading (uplevel)     |
| <kbd>ctrl</kbd> + <kbd>shift</kbd> + <kbd>[</kbd> | Toggle heading (downlevel)   |
| <kbd>alt</kbd> + <kbd>c</kbd>                     | Check/Uncheck task list item |

## Available Commands

- Markdown: Create Table of Contents
- Markdown: Update Table of Contents
- Markdown: Toggle code span
- Markdown: Toggle strikethrough
- Markdown: Print current document to HTML

## Supported Settings

| Name                                               | Default   | Description                                                                        |
| -------------------------------------------------- | --------- | ---------------------------------------------------------------------------------- |
| `markdown.extension.toc.levels`                    | `1..6`    | Control the heading levels to show in the table of contents.                       |
| `markdown.extension.toc.unorderedList.marker`      | `-`       | Use `-`, `*` or `+` in the table of contents (for unordered list)                  |
| `markdown.extension.toc.orderedList`               | `false`   | Use ordered list in the table of contents.                                         |
| `markdown.extension.toc.plaintext`                 | `false`   | Just plain text.                                                                   |
| `markdown.extension.toc.updateOnSave`              | `false`   | Automatically update the table of contents on save.                                |
| `markdown.extension.toc.encodeUri`                 | `true`    | You might want to set this to `false` if you have some non-Latin characters in TOC |
| `markdown.extension.preview.autoShowPreviewToSide` | `false`   | Automatically show preview when opening a Markdown file.                           |
| `markdown.extension.orderedList.marker`            | `ordered` | Or `one`: always use `1.` as ordered list marker                                   |
| `markdown.extension.italic.indicator`              | `*`       | Use `*` or `_` to wrap italic text                                                 |
| `markdown.extension.quickStyling`                  | `false`   | Toggle bold/italic without selecting words                                         |
| `markdown.extension.showExplorer`                  | `true`    | Show outline view in explorer panel                                                |
| `markdown.extension.print.absoluteImgPath`         | `true`    | Convert image path to absolute path                                                |

## Changelog

### 1.1.0 (2018.03.08)

- **New**: Option `toc.encodeUri` ([#90](https://github.com/neilsustc/vscode-markdown/issues/90), [#98](https://github.com/neilsustc/vscode-markdown/issues/98))
- **Fix**: TOC detection ([#85](https://github.com/neilsustc/vscode-markdown/issues/85), [#102](https://github.com/neilsustc/vscode-markdown/issues/102))
- **Fix**: Wrong HTML output path if you are editing `.MD` file ([#105](https://github.com/neilsustc/vscode-markdown/issues/105))

See [CHANGELOG](CHANGELOG.md) for more information.

## Contributing

Bugs, feature requests and more, in [GitHub Issues](https://github.com/neilsustc/vscode-markdown/issues).

Or leave a review on [vscode marketplace](https://marketplace.visualstudio.com/items?itemName=yzhang.markdown-all-in-one#review-details) 😉.
