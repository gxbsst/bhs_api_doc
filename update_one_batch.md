# 更新Batch信息

### 说明
该API使用在检测零件时， 当检测完成某个批次，更新batch的状态

当检测完某batch时，状态转换为`packaged`->`inspected`

### URL

`http://host/api/iqc/batches/<batch_id>?database=<database>&access_token=<access_token>`

##### HTTP 方法:

PATCH

#####参数详细:

**database**: 当前openerp启动使用的数据名字, 请咨询API开发者。

**access_token**:  用户登陆token， 请咨询API开发者

**package_id"**:  package id

**state**: batch总共有四种状态(`draft`, `packaging`, `packaged`, `inspected`)



** 返回 **:

参考一下

``` json
{
    "inspection_quantity": false,
    "order_no": "1",
    "pos": "1",
    "arrival_date_str": "20121011",
    "is_sampling": false,
    "id": 22,
    "work_no": 1,
    "ok_quantity": 1,
    "state": "inspected",
    "ng_quantity": 1,
    "supplier": {
        "name": "name 1",
        "no": "123456"
    },
    "is_urgent": false,
    "inspection_datetime": null,
    "quantity": 1
}
```
