### 学习任务

- 替换字符串 

  #### 替换命令 :substitute

    ##### 公式 :[range(范围)]s[ubstitute(命令)]/{pattern(查找的内容|支持正则)}/{string(要替换的内容)}/[flags()]
      
    > `:s/vnode/node + enter` 查找 `vnode` 替换为 `node`


  ##### rang

    - 范围

      - `$` 到尾部
      > `:10,$s/vnode/node` 从第 10 行开始向后查找 `vnode` 替换为 `node`

      - `%` 全文
      
      - `number,number`

    abc
  
    abc abc

    abc abcabc