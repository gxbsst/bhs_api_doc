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
        "description": "1111",
        "fail_code_description": "description",
        "fail_code_id": 2,
        "fail_code_code": "name 3",
        "part_id": 9,
        "measurement": 111,
        "id": 1,
        "ng_qty": 11,
        "fail_code_name": "name 3",
        "inspection_id": 1,
        "batch_id": 22,
        "inspector_id": 8,
        "rule_id": 1
    }
]

```
