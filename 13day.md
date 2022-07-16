### 学习任务

- 替换字符串 

  #### 替换命令 :substitute

    ##### 公式
      
    > [range]s[ubstitute]/{pattern(查找的内容|支持正则)}/{string(要替换的内容)}/[flags]


    ##### rang

    - 范围

      - `$` 到尾部
        > `:10,$s/vnode/node + enter` 从第 10 行开始向后全文查找每行第一个匹配的 `vnode` 替换为 `node`

      - `%` 全文
        > `:%s/vnode/node + enter` 全文查找每行第一个匹配到的 `vnode` 替换为 `node`
      
      - `number,number + enter` 查找第10行到第20之间每行第一个匹配到的 `vnode` 替换为 `node`
        > `:10,20s/vnode/node`

    ##### flag 

    - `g` 用于全局匹配
      > `:%s/vnode/node/g + enter` 全局匹配 `vnode` 替换为 `node`

    - `c` 弹出对话框，选择替换方式
      > `:%s/vnode/node/[g]c + enter` 弹出对话框
    
      - y 替换当前高亮的
      - n 跳过当前高亮的
      - a 全部替换
      - q 退出
      - l 替换退出

    ##### 可视化模式下

    > `进行可视化模式 + :s/vnode/node/g` 在选中的范围内容进行替换

  #### 查看帮助文档

  > 进入 `vim` 编辑器，键入 `:help s_flags + enter` 

  #### 多选操作

  - `gb`
    > 查找当前所在光标最近的单词(区分大小写)



    abc
  
    abc abc

    abc abcabc