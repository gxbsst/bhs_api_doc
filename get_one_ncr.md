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
    "inspector_name": "杨书超",
    "inspection_logs": [
        {
            "status": "ng",
            "ng_qty": "",
            "description": "",
            "order_no": "0134799",
            "part_no": "10002",
            "fail_code_name": "",
            "fail_code_id": "",
            "pos": "001",
            "rule": {
                "reference_value": "",
                "tool": "工具1",
                "standard": 11,
                "down": 10,
                "step": 1,
                "part_id": 13,
                "id": 1,
                "unit": "mm",
                "name": "步骤1",
                "coord_y": 21,
                "coord_x": 11,
                "standard_str": "",
                "up": 15,
                "type": "quantitative"
            },
            "fail_code_description": "",
            "package_id": "",
            "inspection_id": 4,
            "fail_code_code": "",
            "part_id": 13,
            "measurement": 1,
            "batch_id": 12,
            "inspector_id": 24,
            "id": 4,
            "ncr_id": 4
        }
    ],
    "inspection": {
        "batch_id": 12,
        "ok_quantity": 0,
        "ng_quantity": 1,
        "id": 4
    },
    "id": 4,
    "batch": {
        "work_no": 1,
        "inspection_quantity": 100,
        "packaged_quantity": 157,
        "order_no": "0134799",
        "state": "draft",
        "ok_quantity": 50,
        "pos": "001",
        "inspection_datetime": null,
        "arrival_date_str": "20121011",
        "part": {
            "remark": "Remark....",
            "image_medium": "/api/iqc/part_images/13?size=medium",
            "instruction_image": "/api/iqc/part_instruction_images/13",
            "name": "压板",
            "no": "17815110",
            "rules": [
                {
                    "reference_value": "",
                    "tool": "工具1",
                    "standard": 11,
                    "down": 10,
                    "step": 1,
                    "part_id": 13,
                    "id": 1,
                    "unit": "mm",
                    "name": "步骤1",
                    "coord_y": 21,
                    "coord_x": 11,
                    "standard_str": "",
                    "up": 15,
                    "type": "quantitative"
                },
                {
                    "reference_value": "",
                    "tool": "工具2",
                    "standard": 1,
                    "down": 11,
                    "step": 2,
                    "part_id": 13,
                    "id": 2,
                    "unit": "mm",
                    "name": "步骤2",
                    "coord_y": 21,
                    "coord_x": 11,
                    "standard_str": "",
                    "up": 15,
                    "type": "quantitative"
                },
                {
                    "reference_value": "",
                    "tool": "工具3",
                    "standard": 11,
                    "down": 10,
                    "step": 3,
                    "part_id": 13,
                    "id": 3,
                    "unit": "mm",
                    "name": "步骤3",
                    "coord_y": 21,
                    "coord_x": 11,
                    "standard_str": "",
                    "up": 15,
                    "type": "quantitative"
                }
            ],
            "image": "/api/iqc/part_images/13?size=big",
            "unit_en": "package",
            "image_small": "/api/iqc/part_images/13?size=small",
            "machine": "DFC",
            "c3": "E",
            "c2": "Small Parts",
            "name_en": "name en 1",
            "c1": "M",
            "id": 13,
            "unit": "package",
            "c4": "A"
        },
        "ng_quantity": 50,
        "supplier": {
            "name": "杭州共拓机电有限公司",
            "no": "4300231"
        },
        "is_urgent": false,
        "is_sampling": false,
        "id": 12,
        "quantity": 100
    }
}

```
