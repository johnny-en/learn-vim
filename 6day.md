### 学习任务

- 认识文本对象

  > 文本是结构化，可快速选择

- 语法

    - operator(动作) + 内|外部 + 文本对象

    - 可视化模式 + 内|外部 + 文本对象

- 内部: `i`

- 外部: `a`

- 文本对象

    - `(` 或 `)` 
    
    - `b` 一对 `()`
      
      > `v - i - (|)` 选择 `()` 内部的文本
        `v - a - (|)` 选择 `()` 外部的文本

    - `w` 

      > `d - i - w` 删除光标所在范围的单词  
        `d - a - w` 如果单词前后有空格，优先选中单位后面的空格，否则选中单词前端的空格并删除单词

    - `[` 或 `]`

    - `<` 或 `>`

    - `{` 或 `}` 
    
    - `B` 一对 `{}`

    - `

    - `"`

    - `'`
    - `t`: 表示 `xml` 标签

      > `v - i - t` 选中 `xml` 标签内部的文本

      > `d - a - t` 删除整个 `xml` 标签

    - `s`: 一个句子

    - `p`: 一个段落

- `vim-textobj-arguments`: `vscode` 集成的 `vim` 处理函数的参数
  
    - `ia` 不包含分隔符

    > `daa` 删除一个参数
  
    - `aa` 包含分隔符

    > `cia` 修改一个参数


- `vim-textobj-entire`

  - `dae` 删除当前文本所有内容

  - `die` 删除当前文本所有内容，但是不包含前端和后面的空格