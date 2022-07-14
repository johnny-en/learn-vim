### 学习任务

- 处理包裹字符的符号 

  #### vim surround

    - `c - s - existing(存在的符号) - desired(要替换的符号)` change existing surround to desired
      > `c - s - " - '` 将 `"` 包裹的字符符号替换成 `'` 

    - `y - s - motion(范围) - desired(要包裹的符号)` add desired surround around text defined by
      > `y - s - iw - {` 将单词使用 `{}` 包裹

    - `d - s - existing(存在的符号)` delete existing surround
      > `d - s - [` 删除 `[]` 包裹的符号

    - `S - desired(要包裹的符号)` surround when in visual modes (surrounds full selection)
      > `v - motion(选择范围) - S - "` 在可视化模式选择要包裹的内容，使用 `"` 包裹  
  