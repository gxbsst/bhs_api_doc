# 获取某个批次的NCR信息

### URL

`http://host/api/iqc/ncrs/<batch_id>/?database=<database>&access_token=<access_token>`

##### HTTP 方法:
GET

#####参数详细:

**database**: 当前openerp启动使用的数据名字, 请咨询API开发者。

**access_token**:  用户登陆token， 请咨询API开发者

**batch_id**:  某批次的id(batch id)

** 返回 **:

参考一下

``` json
{
    "ncr_items": [
        {
            "fail_code": {
                "description": "description",
                "code": 1,
                "id": 2,
                "name": "name 3"
            },
            "inspection_log": {
                "status": "ng",
                "description": false,
                "order_no": "1",
                "part_no": "1",
                "pos": "1",
                "package_id": false,
                "part_id": 1,
                "measurement": 0,
                "inspection_id": 9,
                "batch_id": 3,
                "inspector_id": 1,
                "rule_id": 1
            },
            "id": 5,
            "ncr_id": 5
        }
    ],
    "inspection": [
        {
            "batch_id": 3,
            "ok_quantity": 2,
            "ng_quantity": 24,
            "id": 9
        }
    ],
    "id": 5,
    "batch": {
        "work_no": 1,
        "inspection_quantity": 1,
        "arrival_date": "2012-10-11 19:00:00",
        "order_no": "1",
        "part_no": "1",
        "ok_quantity": 1,
        "supplier_no": "1",
        "pos": "1",
        "state": "packaged",
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
        "id": 3,
        "quantity": 1
    }
}


```
