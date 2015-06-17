### URL

`http://host/api/iqc/locations/actions/continue_last_action?database=<database>&access_token=<access_token>`

##### HTTP 方法:
POST

#####参数详细:

**database**: 当前openerp启动使用的数据名字, 请咨询API开发者。

**access_token**:  用户登陆token， 请咨询API开发者

#####表单参数:

**location_name**: 可选参数，库位名如: 1-1-1。

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
        "batch": {
            "inspection_quantity": false,
            "order_no": false,
            "pos": false,
            "arrival_date_str": "",
            "part": {},
            "is_sampling": false,
            "id": 0,
            "work_no": false,
            "ok_quantity": false,
            "state": false,
            "ng_quantity": false,
            "supplier": {
                "name": false,
                "no": false
            },
            "is_urgent": false,
            "inspection_datetime": null,
            "quantity": false
        },
        "state": false,
        "qr_code": "",
        "id": 0,
        "quantity": false
    },
    "id": 1
}

```
