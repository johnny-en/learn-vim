### 学习任务
- 移动到行首
    
  1. `0` 移动到行首

  2. `^` 移动到当前行第一个不是`blank`[^1]的字符
  
        > 改键[^2]：`H`

- 移动到行尾

  1. `$` 移动到行尾
  
  2. `g_` 移动到行尾不是`blank`的字符
    
        > 改键：`L`

- 行首插入
  
  - `I` 移动到行首进行插入

- 行前插入  
  
  - `O` 在当前行的上一行进行插入

- 行尾插入

  - `A` 移动到行尾进行插入

- 行后插入

  - `o` 在当前行的下一行进行插入

- 复制

  - `yy`[^3] 复制当前行

- 粘贴

  - `p` 粘贴复制的行

- 删除

  - `dd` 删除当前行



  [^1]: tab、空格、换行、回车等

  [^2]: 为了减少手指的移动距离，在 `settings.json` 配置 `vim.normalModeKeyBindings` 做重新映射

  [^3]: 此复制的内容单独存储在一个容器中，和 `ctrl c` 复制的内容不冲突