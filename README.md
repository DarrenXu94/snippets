# Snippets

A set of my own personal snippets I use

## How to use

Ctrl + Shift + P and search for snippets

Search for typescriptreact

Copy the relevant files over to the relevant extensions

## Snippets

```
func
```

```
import React from 'react'

export interface ${TM_FILENAME_BASE}Props {
}

export default function ${TM_FILENAME_BASE}() {
  return (
    <div>

    </div>
  )
}
```

## Personal Reference

| TM_SELECTED_TEXT | The currently selected text or the empty string             |
| ---------------- | ----------------------------------------------------------- |
| TM_CURRENT_LINE  | The contents of the current line                            |
| TM_CURRENT_WORD  | The contents of the word under cursor or the empty string   |
| TM_LINE_INDEX    | The zero-index based line number                            |
| TM_LINE_NUMBER   | The one-index based line number                             |
| TM_FILENAME      | The filename of the current document                        |
| TM_FILENAME_BASE | The filename of the current document without its extensions |
| TM_DIRECTORY     | The directory of the current document                       |
| TM_FILEPATH      | The full file path of the current document                  |
| CLIPBOARD        | The contents of your clipboard                              |
| WORKSPACE_NAME   | The name of the opened workspace or folder                  |
