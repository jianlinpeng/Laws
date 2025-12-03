```base
filters:
  or:
    - file.hasTag("最高法指导性案例")
    - file.hasTag("最高检指导性案例")
views:
  - type: table
    name: 指导性案例
    order:
      - file.name
      - 案件类型
      - 罪名
      - 审理程序
      - 入库编号
      - 入库日期
      - 裁定法院
      - 裁定日期
      - file.mtime
      - 文号
    sort:
      - property: 文号
        direction: ASC
      - property: 裁定日期
        direction: ASC
    columnSize:
      file.name: 285
      note.案件类型: 94
      note.罪名: 108
      note.审理程序: 89
      note.入库编号: 150
      note.入库日期: 97
      note.裁定法院: 174
      file.mtime: 96
      note.文号: 251
  - type: table
    name: 最高法指导性案例
    filters:
      and:
        - file.hasTag("最高法指导性案例")
    order:
      - file.name
      - 案件类型
      - 罪名
      - 审理程序
      - 入库编号
      - 入库日期
      - 裁定法院
      - 裁定日期
      - file.mtime
      - 文号
    sort:
      - property: file.name
        direction: ASC
      - property: 文号
        direction: ASC
      - property: 裁定日期
        direction: ASC
    columnSize:
      file.name: 285
      note.案件类型: 94
      note.罪名: 108
      note.审理程序: 89
      note.入库编号: 150
      note.入库日期: 97
      note.裁定法院: 174
      file.mtime: 96
      note.文号: 251
  - type: table
    name: 最高检指导性案例
    filters:
      and:
        - file.hasTag("最高检指导性案例")
    order:
      - file.name
      - 案件类型
      - 罪名
      - 审理程序
      - 入库编号
      - 入库日期
      - 裁定法院
      - 裁定日期
      - file.mtime
      - 文号
    sort:
      - property: 文号
        direction: ASC
      - property: 裁定日期
        direction: ASC
    columnSize:
      file.name: 285
      note.案件类型: 94
      note.罪名: 108
      note.审理程序: 89
      note.入库编号: 150
      note.入库日期: 97
      note.裁定法院: 174
      file.mtime: 96
      note.文号: 251

```
