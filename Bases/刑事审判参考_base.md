```base
filters:
  and:
    - file.hasTag("刑事审判参考")
views:
  - type: table
    name: 刑事审判参考
    order:
      - file.name
      - 发布日期
      - 施行日期
      - 发文机关
    columnSize:
      file.name: 415
      note.发布日期: 127
      note.施行日期: 111

```
