# Snippets

A set of my own personal snippets I use

## How to use

Ctrl + Shift + P and search for snippets

Search for typescriptreact

Copy the relevant files over to the relevant extensions

## Snippets

- [`func`](#-func-)
- [`usef`](#-usef-)
- [`storybook`](#-storybook-)
- [`usehook`](#-usehook-)
- [`uses`](#-uses-)
- [`backquote`](#-backquote-)

<a name="-func-"> </a>

### `func`

```
import React from 'react'

export interface ${TM_FILENAME_BASE}Props {
    $0
}

export default function ${TM_FILENAME_BASE}({}: ${TM_FILENAME_BASE}Props) {
  return (
    <div>

    </div>
  )
}
```

<a name="-usef-"> </a>

### `usef`

```
useEffect(() => {
  $2
}, [$1]);
```

<a name="-storybook-"> </a>

### `storybook`

```
import React from "react";
import ${TM_FILENAME_BASE/(.*)\\..+$/$1/}, {${TM_FILENAME_BASE/(.*)\\..+$/$1/}Props} from "./${TM_FILENAME_BASE/(.*)\\..+$/$1/}";
import { Meta, Story } from "@storybook/react";

export default {
  title: "${TM_FILENAME_BASE/(.*)\\..+$/$1/}",
} as Meta;

const Template: Story<${TM_FILENAME_BASE/(.*)\\..+$/$1/}Props> = (args) => {
  return <${TM_FILENAME_BASE/(.*)\\..+$/$1/} {...args} />;
};

export const Primary = Template.bind({});
Primary.args = {
  $0
};
```

<a name="-usehook-"> </a>

### `usehook`

```
export default function ${TM_FILENAME_BASE/(.*)\\..+$/$1/}() {
  const func = async () => {
    $0
  };

  return { func };
}
```

<a name="-uses-"> </a>

### `uses`

```
const [${1}, set${1/(.*)/${1:/capitalize}/}] = useState(${2})
```

<a name="-backquote-"> </a>

### `$`

```
\\${$1}
```

## Personal Reference

[Snippet generator](https://snippet-generator.app/?description=&tabtrigger=&snippet=&mode=vscode)

| Variable         | Description                                                 |
| ---------------- | ----------------------------------------------------------- |
| TM_SELECTED_TEXT | The currently selected text or the empty string             |
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
