# 更新Package信息

### 说明
该API使用在检测零件时， 当扫描某个package时， 将package的状态(`state`)从`draft`->`inspecting`

当检测完某package时，状态转换为`inspecting`->`inspected`

### URL

`http://host/api/iqc/packages/<package_id>?database=<database>&access_token=<access_token>`

##### HTTP 方法:

PATCH

#####参数详细:

**database**: 当前openerp启动使用的数据名字, 请咨询API开发者。

**access_token**:  用户登陆token， 请咨询API开发者

**package_id"**:  package id

**state**: package总共有三种状态(`draft`, `inspecting`, `inspected`)



** 返回 **:

参考一下

``` json
{
    "batch": {
        "work_no": 1,
        "inspection_quantity": 1,
        "arrival_date": "2012-10-11 19:00:00",
        "order_no": "1",
        "part_no": "1",
        "ok_quantity": 1,
        "supplier_no": "1",
        "pos": "1",
        "state": "draft",
        "part": {
            "remark": "Remark....",
            "image_medium": "/api/iqc/part_images/5?size=medium",
            "name": "name 1",
            "instruction_image": "/api/iqc/part_instruction_images/5",
            "rules": [
                {
                    "tool": "tool",
                    "standard": 11,
                    "down": 10,
                    "step": 1,
                    "part_id": 5,
                    "id": 1,
                    "name": "name 1",
                    "coord_y": 21,
                    "coord_x": 11,
                    "up": 15,
                    "type": "quantitative"
                },
                {
                    "tool": "tool",
                    "standard": 1,
                    "down": 11,
                    "step": 2,
                    "part_id": 5,
                    "id": 2,
                    "name": "name 1",
                    "coord_y": 21,
                    "coord_x": 11,
                    "up": 15,
                    "type": "quantitative"
                },
                {
                    "tool": "tool",
                    "standard": 11,
                    "down": 10,
                    "step": 3,
                    "part_id": 5,
                    "id": 3,
                    "name": "name 1",
                    "coord_y": 21,
                    "coord_x": 11,
                    "up": 15,
                    "type": "quantitative"
                }
            ],
            "c3": "c3",
            "c2": "c2",
            "name_en": "name en 1",
            "c1": "c1",
            "unit": "package",
            "c4": "c4",
            "remark": "Remark....",
            "name": "name 1",
            "unit_en": "package",
            "id": 2,
            "machine": "machine name"
        },
        "ng_quantity": 1,
        "inspection_datetime": false,
        "supplier": {
            "name": "name 1",
            "no": "123456"
        },
        "is_urgent": false,
        "id": 2,
        "quantity": 1
    },
    "state": "draft",
    "qr_code": "1111",
    "id": 2,
    "quantity": 10
}
```
