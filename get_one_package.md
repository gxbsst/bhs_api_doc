# 获取某个package

### URL

`http://host/api/iqc/packages/<qr_code>/?database=<database>&token=<access_token>`

##### HTTP 方法:
GET

#####参数详细:

**database**: 当前openerp启动使用的数据名字, 请咨询API开发者。

**access_token**:  用户登陆token， 请咨询API开发者
**qr_code**: package的qr_code

** 返回 **:

参考一下

``` json

{
    "qr_code": "1111",
    "batch": {
        "work_no": 1,
        "inspection_quantity": 1,
        "arrival_date": "2012-10-11 19:00:00",
        "order_no": "1",
        "part_no": "12",
        "ok_quantity": 1,
        "instruction": {
            "name": "name 1",
            "file": null
        },
        "supplier_no": "1",
        "pos": "1",
        "rules": [
            {
                "tool": "tool",
                "standard": 1,
                "down": 0,
                "step": 1,
                "part_id": 1,
                "id": 1,
                "name": "name 1",
                "coord_y": 21,
                "coord_x": 11,
                "up": 0,
                "type": "quantitative"
            },
            {
                "tool": "tool",
                "standard": 1,
                "down": 0,
                "step": 2,
                "part_id": 1,
                "id": 2,
                "name": "name 1",
                "coord_y": 21,
                "coord_x": 11,
                "up": 0,
                "type": "quantitative"
            },
            {
                "tool": "tool",
                "standard": 1,
                "down": 0,
                "step": 3,
                "part_id": 1,
                "id": 3,
                "name": "name 1",
                "coord_y": 21,
                "coord_x": 11,
                "up": 0,
                "type": "quantitative"
            }
        ],
        "state": "draft",
        "part": {
            "instruction_id": 2,
            "c3": "c3",
            "c2": "c2",
            "name_en": "name en 1",
            "c1": "c1",
            "unit": "package",
            "c4": "c4",
            "remark": "Remark....",
            "name": "name 1",
            "unit_en": "package",
            "id": 1,
            "machine": "machine name"
        },
        "ng_quantity": 1,
        "inspection_datetime": false,
        "supplier": {
            "name": "name 1",
            "no": "123456"
        },
        "is_urgent": false,
        "inspector": {},
        "id": 1,
        "quantity": 1
    },
    "state": "draft",
    "batch_id": 1,
    "id": 1,
    "quantity": 10
}


```
