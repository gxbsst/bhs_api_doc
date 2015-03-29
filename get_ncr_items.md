# 获取NCR Items

### URL

`http://host/api/iqc/ncr_items?database=<database>&access_token=<access_token>`

##### HTTP 方法:
GET

#####参数详细:

**database**: 当前openerp启动使用的数据名字, 请咨询API开发者。

**access_token**:  用户登陆token， 请咨询API开发者

**ncr_id**: 如果需要获取某条ncr的所有items， 则需要给出ncr_id, 否则返回全部

** 返回 **:

参考一下

``` json

[
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
    },
    {
        "fail_code": {
            "description": false,
            "code": false,
            "id": 0,
            "name": false
        },
        "inspection_log": {
            "status": "ng",
            "description": "hello....",
            "order_no": "1",
            "part_no": "1",
            "pos": "1",
            "package_id": 2,
            "part_id": 1,
            "measurement": 10.02,
            "inspection_id": 9,
            "batch_id": 3,
            "inspector_id": 1,
            "rule_id": 1
        },
        "id": 6,
        "ncr_id": 5
    }
    ]

```
