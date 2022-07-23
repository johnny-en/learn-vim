### 学习任务

#### `vim` 调用 `vscode` 的命令

##### 格式化文档

- `shift + alt + f` 格式化文档

> 在首选项添加配置

```json
   "vim.normalModeKeyBindingsNonRecursive": [
        {
            "before":["<leader>","f","d"],
            "commands":[ "editor.action.formatDocument" ]
        },
   ]
```

- `F2` 重命名

```json
  "vim.normalModeKeyBindingsNonRecursive": [
      {
          "before":["<leader>","r","n"],
          "commands":[ "editor.action.rename" ]
      },
  ]
```

- `C + shift + [` 代码折叠

```json
  "vim.normalModeKeyBindingsNonRecursive": [
    {
        "before":["<leader>","["],
        "commands":[ 
            {
                "command": "editor.fold",
            },
            // 触发折叠光标会跳转到行尾，键入 J 会展开代码，所以加入 vim 指令在折叠后光标跳转到下一行
            {
                "command": "vim.remap",
                "args":{
                    "after":["$","%"]
                }
            }
        ]
    },
  ]
```

