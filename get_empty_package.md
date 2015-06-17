# 获取一个空箱

### URL

`http://host/iqc/locations/actions/pull_empty?database=<database>&access_token=<access_token>`

##### HTTP 方法:
POST

#####参数详细:

**database**: 当前openerp启动使用的数据名字, 请咨询API开发者。

**access_token**:  用户登陆token， 请咨询API开发者

** 返回 **:

参考一下

``` json

{
    "pos_z": 1,
    "pos_x": 1,
    "pos_y": 1,
    "name": "111",
    "state": "full",
    "active": true,
    "package": {
        "batch": {},
        "state": false,
        "qr_code": "",
        "id": 0,
        "quantity": 0
    },
    "id": 1
}

```
