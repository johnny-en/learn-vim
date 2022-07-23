### 学习任务

#### 操作文件 

##### 切换到 `files explorer`(资源管理器) 区域 

- `ctrl + shift + e` 格式化文档

    > 在键盘快捷方式添加配置

    ```json
    {
    "key": "ctrl+;",
    "command": "workbench.view.explorer",
    "when": "viewContainer.workbench.view.explorer.enabled"
    }

    ```

- `ctrl + 1` 切换到编辑区域

    ```json
    {
    "key": "ctrl+'",
    "command": "workbench.action.focusFirstEditorGroup"
    }
    ```

##### 移动光标 `hjkl`

##### 折叠/展开 `h/l`

##### 创建文件

    1. `a` 在资源管理器下使用快捷键

        ```json
        {
            "key": "a",
            "command": "explorer.newFile",
            "when": "filesExplorerFocus && !inputFocus"
        }
        ```
    2. `leader + n + f` 在编辑模式下，在首选项添加配置

        ```json
        "vim.normalModeKeyBindingsNonRecursive": [
            {
                "before":["<leader>","n","f"],
                "commands":["explorer.newFile"]
            },
        ]
        ```
    3. 使用 `vscode` `ctrl + n`
    4. 使用 `file utils` 插件

##### 创建文件夹

    1. `A` 在资源管理器下使用快捷键

        ```json
        {
            "key": "shift+a",
            "command": "explorer.newFolder",
            "when": "filesExplorerFocus && !inputFocus"
        }
        ```
    2. `leader + n + f` 在编辑模式下，在首选项添加配置

        ```json
        "vim.normalModeKeyBindingsNonRecursive": [
            {
                "before":["<leader>","n","d"],
                "commands":["explorer.newFolder"]
            },
        ]
        ```
    3. 使用 `file utils` 插件

##### 重命名

    ```json
    {
        "key": "r",
        "command": "renameFile",
        "when": "explorerViewletVisible && filesExplorerFocus && !explorerResourceIsRoot && !explorerResourceReadonly && !inputFocus"
    }
    ```
##### 删除

    ```json
    {
        "key": "d",
        "command": "deleteFile",
        "when": "explorerViewletVisible && filesExplorerFocus && !explorerResourceIsRoot && !explorerResourceReadonly && !inputFocus"
    }
    ```