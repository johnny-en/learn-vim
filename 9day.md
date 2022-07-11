### 学习任务

- 更高效的移动-任意跳转

- vim-easymotion

  > `vscode vim` 已经集成，只需要通过配置开启此功能

  - 基于单词快速跳转 

      - `<leader> - <leader> - w` 从当前光标向后高亮词首 
      
      - `<leader> - <leader> - b` 从当前光标向前高亮词首 

      - `<leader> - <leader> - e` 从当前光标向后高亮词尾 

      - `<leader> - <leader> - ge` 从当前光标向前高亮词尾

      - `<leader> - <leader> - l` 从当前光标向后高亮词首/尾

      - `<leader> - <leader> - h` 从当前光标向后高亮词首/尾

  - 基于行快速跳转

      - `<leader> - <leader> - j` 从当前光标向后高亮行首
      
      - `<leader> - <leader> - k` 从当前光标向前高亮行首

  - 任意快速跳转

      - `<leader> - <leader> - <leader> - j` 

- vim-sneak
  
   > `vscode vim` 已经集成，只需要通过配置开启此功能

  - `s + 2个字符` 实现快速跳转
  
  - 改键 

    - 替换原生的 `f` 功能

    - 利用映射来实现原有的 `s/S/z/Z`

    - `v + f + 2char`

    - `operation + z + 2char`