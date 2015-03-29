# 获取检测错误代码

# 获取NCR Items

### URL

`http://host/api/iqc/fail_codes?database=<database>&access_token=<access_token>`

##### HTTP 方法:
GET

#####参数详细:

**database**: 当前openerp启动使用的数据名字, 请咨询API开发者。

**access_token**:  用户登陆token， 请咨询API开发者


** 返回 **:

参考一下

``` json

[
    {
        "description": "description",
        "code": 1,
        "id": 1,
        "name": "name 1"
    },
    {
        "description": "description",
        "code": 1,
        "id": 2,
        "name": "name 3"
    },
    {
        "description": "description",
        "code": 3,
        "id": 3,
        "name": "name 3"
    }
]

```
