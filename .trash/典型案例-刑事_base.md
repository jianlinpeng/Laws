```base
filters:
  and:
    - file.inFolder("典型案例/10 刑事")
views:
  - type: table
    name: 表格
    order:
      - file.name
      - 罪名
      - 审理程序
      - 入库编号
      - 入库日期
      - 裁定日期
      - 裁定法院
      - 修改日期
      - 文号
    sort:
      - property: 入库编号
        direction: ASC
    columnSize:
      file.name: 360
      note.罪名: 125
      note.审理程序: 90
      note.入库编号: 150
      note.入库日期: 100
      note.裁定法院: 110
      note.修改日期: 90
      note.文号: 230
  - type: table√
    name: 视图
  - type: table
    name: 视图 2

```
