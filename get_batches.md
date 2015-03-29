# 获取批次

### URL

`http://host/api/iqc/batches?database=<database>&access_token=<access_token>&state=<state>&offset=<offset>&limit=<limit>`

##### HTTP 方法:
GET

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
        "inspection_quantity": 0,
        "order_no": "1",
        "pos": "1",
        "part": {
            "remark": false,
            "image_medium": null,
            "name": "测试零件",
            "rules": [],
            "image": null,
            "unit_en": false,
            "image_small": null,
            "machine": false,
            "instruction": {},
            "c3": false,
            "c2": false,
            "name_en": false,
            "c1": false,
            "id": 2,
            "unit": false,
            "c4": false
        },
        "id": 4,
        "work_no": 0,
        "arrival_date": false,
        "ok_quantity": 0,
        "state": "draft",
        "ng_quantity": 0,
        "supplier": {
            "name": "测试供应商",
            "no": "1"
        },
        "is_urgent": false,
        "inspection_datetime": false,
        "quantity": 0
    }
]

```
