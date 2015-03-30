# 更新库位状态
### URL

`http://host/iqc/locations/<location_id>?database=<database>&access_token=<access_token>`

##### HTTP 方法:
PATCH

#####URL参数:

**location_id**: 库位id。

**database**: 当前openerp启动使用的数据名字, 请咨询API开发者。

**access_token**:  用户登陆token， 请咨询API开发者

#####表单参数:

**state**: 需要更新的状态值，取empty或者full。

**package_id**: 在存放货物的时候需要提供此字段，清空库位的时候无需提供。

** 返回 **:

参考一下

``` json

{
    "pos_z": 1,
    "pos_x": 1,
    "pos_y": 1,
    "name": "111",
    "state": "empty",
    "active": true,
    "package": {},
    "id": 1
}

```
