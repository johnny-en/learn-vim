### 学习任务

#### 如何删除一个函数

##### `%` 匹配括号
    > `v - %` 光标在 `( | { | [` 上按 `v` 进入可视化模式，再按 `%` 可快速选中闭合标签

##### vim-indent-object
> 通过对 `vim` 配置可以简化操作项

  - `vii` 选中函数内部内容, 函数内执行
  - `vai` 选中整个函数，但不包括最后的大括号，函数内执行
  - `vaI` 选中整个函数，函数内执行

##### 删除方式
> 通过对 `vim` 配置可以简化操作项

  - `dap` 基于段落删除, 函数内执行
  - `daI` 删除整个函数, 函数内执行
  - `V$%` 选中整个函数，函数声明所在行执行

