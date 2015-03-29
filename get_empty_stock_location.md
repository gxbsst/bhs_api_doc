# 获取一个空库位

### URL

`http://host/iqc/locations?database=<database>&access_token=<access_token>&method=push`

##### HTTP 方法:
GET

#####参数详细:

**database**: 当前openerp启动使用的数据名字, 请咨询API开发者。

**access_token**:  用户登陆token， 请咨询API开发者

**method**: 方式或方法，这里固定取值push（这里表示是为了存放）。

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
    "package_id": false,
    "package": {},
    "id": 1
}

```
