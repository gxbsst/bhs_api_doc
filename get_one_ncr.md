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
    "inspection_logs": [
        {
            "status": "ng",
            "description": "1111",
            "fail_code_description": "description",
            "fail_code_id": 2,
            "fail_code_code": "name 3",
            "part_id": 9,
            "measurement": 111,
            "id": 1,
            "ng_qty": 0,
            "fail_code_name": "name 3",
            "inspection_id": 1,
            "batch_id": 22,
            "inspector_id": 8,
            "rule_id": 1
        }
    ],
    "inspection": [],
    "id": 1,
    "batch": {
        "inspection_quantity": 1,
        "order_no": "1",
        "pos": "1",
        "arrival_date_str": "20121011",
        "part": {
            "remark": "Remark....",
            "image_medium": "/api/iqc/part_images/9?size=medium",
            "instruction_image": "/api/iqc/part_instruction_images/9",
            "name": "name 1",
            "no": "123456",
            "rules": [
                {
                    "reference_value": "",
                    "tool": "tool",
                    "standard": 11,
                    "down": 10,
                    "step": 1,
                    "part_id": 9,
                    "id": 1,
                    "unit": "mm",
                    "name": "name 1",
                    "coord_y": 21,
                    "coord_x": 11,
                    "up": 15,
                    "type": "quantitative"
                },
                {
                    "reference_value": "",
                    "tool": "tool",
                    "standard": 1,
                    "down": 11,
                    "step": 2,
                    "part_id": 9,
                    "id": 2,
                    "unit": "mm",
                    "name": "name 1",
                    "coord_y": 21,
                    "coord_x": 11,
                    "up": 15,
                    "type": "quantitative"
                },
                {
                    "reference_value": "",
                    "tool": "tool",
                    "standard": 11,
                    "down": 10,
                    "step": 3,
                    "part_id": 9,
                    "id": 3,
                    "unit": "mm",
                    "name": "name 1",
                    "coord_y": 21,
                    "coord_x": 11,
                    "up": 15,
                    "type": "quantitative"
                }
            ],
            "image": "/api/iqc/part_images/9?size=big",
            "unit_en": "package",
            "image_small": "/api/iqc/part_images/9?size=small",
            "machine": "machine name",
            "c3": "c3",
            "c2": "c2",
            "name_en": "name en 1",
            "c1": "c1",
            "id": 9,
            "unit": "package",
            "c4": "c4"
        },
        "is_sampling": false,
        "id": 22,
        "work_no": 1,
        "ok_quantity": 1,
        "state": "draft",
        "ng_quantity": 1,
        "supplier": {
            "name": "name 1",
            "no": "123456"
        },
        "is_urgent": false,
        "inspection_datetime": null,
        "quantity": 1
    }
}


```
