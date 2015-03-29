# 创建NCR Item


### URL

`http://host/api/iqc/ncr_items?database=<database>&access_token=<access_token>`

##### HTTP 方法:

POST

#####参数详细:

**database**: 当前openerp启动使用的数据名字, 请咨询API开发者。

**access_token**:  用户登陆token， 请咨询API开发者

**fail_code_id**: fail code id

**ncr_id**: ncr id


** 返回 **:

参考一下

``` json
{
    "fail_code": {
        "description": "description",
        "code": 1,
        "id": 2,
        "name": "name 3"
    },
    "inspection_log": {
        "status": false,
        "description": false,
        "order_no": false,
        "part_no": false,
        "pos": false,
        "package_id": false,
        "part_id": false,
        "measurement": false,
        "inspection_id": false,
        "batch_id": false,
        "inspector_id": false,
        "rule_id": false
    },
    "id": 37,
    "ncr_id": 5
}
```
