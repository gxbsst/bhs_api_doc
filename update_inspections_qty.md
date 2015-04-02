# 更新ok/ng的数量

### 说明
当检测某个零件时，要更新ng或者ok的数量

### URL

`http://host/api/inspections/actions/<batch_id>/update_qty/<status_type>?database=<database>&access_token=<access_token>`

##### HTTP 方法:

PATCH

#####参数详细:

**database**: 当前openerp启动使用的数据名字, 请咨询API开发者。

**access_token**:  用户登陆token， 请咨询API开发者

**batch_id**:  batch_id id

**status_type**: status_type 为`ng` 或者 `ok`



** 返回 **:

参考一下

``` json

{
    "batch_id": 14,
    "ok_quantity": 7,
    "ng_quantity": 8,
    "id": 7
}
```
