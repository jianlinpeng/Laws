```base
filters:
  and:
    - file.inFolder("100 现行有效法律")
    - '!file.inFolder("100 现行有效法律/FZ 废止法律法规")'
    - '!file.hasTag("目录")'
    - '!file.hasTag("修订文件")'
formulas:
  未命名: ""
views:
  - type: table
    name: 现行有效法律
    order:
      - file.name
      - 发文机关
      - 效力级别
      - 发布日期
      - 施行日期
      - 时效性
    sort:
      - property: 施行日期
        direction: DESC
      - property: file.name
        direction: ASC
    columnSize:
      file.name: 256
      note.发文机关: 198
      note.效力级别: 93
      note.发布日期: 125
      note.施行日期: 133
  - type: table
    name: 现行法律-宪法
    filters:
      and:
        - file.inFolder("100 现行有效法律/10 宪法")
    order:
      - file.name
      - 发文机关
      - 效力级别
      - 发布日期
      - 施行日期
      - 时效性
    sort:
      - property: 发布日期
        direction: ASC
      - property: file.name
        direction: ASC
    columnSize:
      file.name: 238
      note.发文机关: 198
      note.效力级别: 93
      note.发布日期: 125
      note.施行日期: 133
  - type: table
    name: 现行法律-宪法相关法
    filters:
      and:
        - file.inFolder("100 现行有效法律/20 宪法相关法")
    order:
      - file.name
      - 发文机关
      - 效力级别
      - 发布日期
      - 施行日期
      - 时效性
    sort:
      - property: 施行日期
        direction: DESC
      - property: file.name
        direction: ASC
    columnSize:
      file.name: 291
      note.发文机关: 198
      note.效力级别: 93
      note.发布日期: 125
      note.施行日期: 133
  - type: table
    name: 现行法律-民法商法
    filters:
      and:
        - file.inFolder("100 现行有效法律/30 民法商法")
    order:
      - file.name
      - 发文机关
      - 效力级别
      - 发布日期
      - 施行日期
      - 时效性
    sort:
      - property: 施行日期
        direction: DESC
      - property: file.name
        direction: DESC
    columnSize:
      file.name: 286
      note.发文机关: 198
      note.效力级别: 93
      note.发布日期: 125
      note.施行日期: 133
  - type: table
    name: 现行法律-行政法
    filters:
      and:
        - file.inFolder("100 现行有效法律/40 行政法")
    order:
      - file.name
      - 发文机关
      - 效力级别
      - 发布日期
      - 施行日期
      - 时效性
    sort:
      - property: 施行日期
        direction: DESC
    columnSize:
      file.name: 288
      note.发文机关: 198
      note.效力级别: 93
      note.发布日期: 125
      note.施行日期: 133
  - type: table
    name: 现行法律-经济法
    filters:
      and:
        - file.inFolder("100 现行有效法律/50 经济法")
    order:
      - file.name
      - 发文机关
      - 效力级别
      - 发布日期
      - 施行日期
      - 时效性
    sort:
      - property: 施行日期
        direction: DESC
    columnSize:
      file.name: 288
      note.发文机关: 198
      note.效力级别: 93
      note.发布日期: 125
      note.施行日期: 133
  - type: table
    name: 现行法律-社会法
    filters:
      and:
        - file.inFolder("100 现行有效法律/60 社会法")
    order:
      - file.name
      - 发文机关
      - 效力级别
      - 发布日期
      - 施行日期
      - 时效性
    sort:
      - property: 施行日期
        direction: DESC
    columnSize:
      file.name: 286
      note.发文机关: 198
      note.效力级别: 93
      note.发布日期: 125
      note.施行日期: 133
  - type: table
    name: 现行法律-刑法
    filters:
      and:
        - file.inFolder("100 现行有效法律/70 刑法")
    order:
      - file.name
      - 发文机关
      - 效力级别
      - 发布日期
      - 施行日期
      - 时效性
    sort:
      - property: 施行日期
        direction: ASC
    columnSize:
      file.name: 283
      note.发文机关: 198
      note.效力级别: 93
      note.发布日期: 125
      note.施行日期: 133
  - type: table
    name: 现行法律-诉讼与非诉讼程序法
    filters:
      and:
        - file.inFolder("100 现行有效法律/80 诉讼与非诉讼程序法")
    order:
      - file.name
      - 发文机关
      - 效力级别
      - 发布日期
      - 施行日期
      - 时效性
    sort:
      - property: 施行日期
        direction: DESC
    columnSize:
      file.name: 277
      note.发文机关: 198
      note.效力级别: 93
      note.发布日期: 125
      note.施行日期: 133

```
