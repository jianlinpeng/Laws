```base
filters:
  or:
    - file.inFolder("典型案例/10 刑事")
    - file.inFolder("典型案例/20 民事")
    - file.inFolder("典型案例/30 行政")
    - file.inFolder("典型案例/40 国家赔偿")
    - file.inFolder("典型案例/50 执行")
views:
  - type: table
    name: 典型案例
    order:
      - file.name
      - 案件类型
      - 罪名
      - 审理程序
      - 入库编号
      - 裁定法院
      - 文号
      - 裁定日期
      - 入库日期
      - 修改日期
    sort:
      - property: 罪名
        direction: ASC
      - property: 文号
        direction: ASC
    columnSize:
      file.name: 209
      note.案件类型: 91
      note.罪名: 203
      note.审理程序: 90
      note.入库编号: 150
      note.裁定法院: 110
      note.文号: 230
      note.入库日期: 100
      note.修改日期: 90
  - type: table
    name: 典型案例-刑事
    filters:
      and:
        - file.inFolder("典型案例/10 刑事")
    order:
      - file.name
      - 罪名
      - 审理程序
      - 入库编号
      - 裁定法院
      - 文号
      - 裁定日期
      - 入库日期
      - 修改日期
    sort:
      - property: 审理程序
        direction: ASC
      - property: 入库编号
        direction: DESC
      - property: 罪名
        direction: DESC
      - property: 文号
        direction: ASC
    columnSize:
      file.name: 233
      note.罪名: 125
      note.审理程序: 89
      note.入库编号: 150
      note.裁定法院: 100
      note.文号: 178
      note.入库日期: 100
      note.修改日期: 90
  - type: table
    name: 典型案例-民事
    filters:
      and:
        - file.inFolder("典型案例/20 民事")
    order:
      - file.name
      - 罪名
      - 审理程序
      - 入库编号
      - 裁定法院
      - 文号
      - 裁定日期
      - 入库日期
      - 修改日期
    sort:
      - property: 入库编号
        direction: ASC
    columnSize:
      file.name: 202
      note.罪名: 125
      note.审理程序: 90
      note.入库编号: 150
      note.裁定法院: 110
      note.文号: 195
      note.入库日期: 100
      note.修改日期: 90
  - type: table
    name: 典型案例-行政
    filters:
      and:
        - file.inFolder("典型案例/30 行政")
    order:
      - file.name
      - 罪名
      - 审理程序
      - 入库编号
      - 裁定法院
      - 文号
      - 裁定日期
      - 入库日期
      - 修改日期
    sort:
      - property: 入库编号
        direction: ASC
    columnSize:
      file.name: 198
      note.罪名: 125
      note.审理程序: 90
      note.入库编号: 150
      note.裁定法院: 110
      note.文号: 203
      note.入库日期: 100
      note.修改日期: 90
  - type: table
    name: 典型案例-国家赔偿
    filters:
      and:
        - file.inFolder("典型案例/40 国家赔偿")
    order:
      - file.name
      - 罪名
      - 审理程序
      - 入库编号
      - 裁定法院
      - 文号
      - 裁定日期
      - 入库日期
      - 修改日期
    sort:
      - property: 审理程序
        direction: DESC
      - property: 入库编号
        direction: ASC
    columnSize:
      file.name: 179
      note.罪名: 140
      note.审理程序: 110
      note.入库编号: 150
      note.裁定法院: 110
      note.文号: 179
      note.入库日期: 100
      note.修改日期: 90
  - type: table
    name: 典型案例-执行
    filters:
      and:
        - file.inFolder("典型案例/50 执行")
    order:
      - file.name
      - 案件类型
      - 罪名
      - 审理程序
      - 入库编号
      - 裁定法院
      - 文号
      - 裁定日期
      - 入库日期
      - 修改日期
    sort:
      - property: 罪名
        direction: DESC
      - property: 入库编号
        direction: ASC
    columnSize:
      file.name: 222
      note.案件类型: 91
      note.罪名: 112
      note.审理程序: 90
      note.入库编号: 150
      note.裁定法院: 110
      note.文号: 189
      note.入库日期: 100
      note.修改日期: 90

```
