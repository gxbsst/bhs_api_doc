# 获取Inspection logs

### 说明

获取某个batch或者所有的检测记录


### URL

`http://host/api/iqc/inspection_logs?database=<database>&access_token=<access_token>`

##### HTTP 方法:
GET

#####参数详细:

**database**: 当前openerp启动使用的数据名字, 请咨询API开发者。

**access_token**:  用户登陆token， 请咨询API开发者

**batch_id**: 如果需要获取某条batch的所有logs， 则需要给出batch_id, 否则返回全部

** 返回 **:

参考一下

``` json

[
    {
        "status": "ng",
        "ng_qty": "",
        "description": "",
        "order_no": "0134799",
        "part_no": "10002",
        "fail_code_name": "",
        "fail_code_id": "",
        "pos": "001",
        "rule_id": {
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
        "inspection_id": 3,
        "fail_code_code": "",
        "part_id": 13,
        "measurement": 1,
        "batch_id": 12,
        "inspector_id": 24,
        "id": 2,
        "ncr_id": 3
    }
]

```
