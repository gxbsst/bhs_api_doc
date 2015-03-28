# 获取批次

### URL

`http://host/api/iqc/batches?database=<database>&access_token=<access_token>&state=<state>&offset=<offset>&limit=<limit>`

##### HTTP 方法:
POST

#####参数详细:

**database**: 当前openerp启动使用的数据名字, 请咨询API开发者。

**access_token**:  用户登陆token， 请咨询API开发者

**state**: 状态，可取：draft,packaging,packaged,inspected
分别对应 初始状态，分拣中，分拣完成，检测完成

**offset**: 偏移多少

**limit**: 限制取多少

** 返回 **:

参考一下

``` json

[
    {
        "work_no": 0,
        "inspection_quantity": 0,
        "arrival_date": false,
        "order_no": "1",
        "part_no": false,
        "ok_quantity": 0,
        "instruction": {},
        "supplier_no": false,
        "pos": "1",
        "rules": [],
        "state": "draft",
        "part": {},
        "ng_quantity": 0,
        "inspection_datetime": false,
        "supplier": {},
        "is_urgent": false,
        "id": 3,
        "quantity": 0
    }
]

```
