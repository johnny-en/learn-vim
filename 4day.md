### 学习任务

- 处理单字符 

  1. 删除光标所在的字符：`x`

  2. 删除光标前的字符：`X`

  3. 删除当前光标的字符并进入 `insert` 模式：`s`

  4. 删除当前光标所在行并进行 `inser` 模式：`S`

  5. 替换一个字符：`r`

  6. 替换多个字符：`R`

- `undo` & `redo`

  > 可撤销块：进入插入模式开始，直到返回普通模式为止，在此期间输入或删除的任务内容都被当成一次修改

  1. `u`

  2. `Ctrl + r`