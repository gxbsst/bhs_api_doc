# 检测员登陆

### URL

`http://host/api/iqc/inspectors/actions/auth?database=<database>&access_token=<access_token>`

##### HTTP 方法:
POST

#####参数详细:

**database**: 当前openerp启动使用的数据名字, 请咨询API开发者。

**access_token**:  用户登陆token， 请咨询API开发者

** 返回 **:

参考一下

``` json

{
    "user_id": 6,
    "qr_code": "login:1427442304299731",
    "id": 1,
    "name": "张三",
    "no": "1"
}

```
