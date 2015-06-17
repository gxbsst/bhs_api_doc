# 获取所有库位信息

### URL

`http://host/api/iqc/locations?database=<database>&access_token=<access_token>`

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
        "pos_z": 1,
        "pos_x": 1,
        "pos_y": 1,
        "name": "1-1-1",
        "state": "empty",
        "active": true,
        "package": {
            "qr_code": "",
            "batch": {
                "work_no": false,
                "inspection_quantity": false,
                "packaged_quantity": false,
                "order_no": false,
                "state": false,
                "ok_quantity": false,
                "pos": false,
                "inspection_datetime": null,
                "arrival_date_str": "",
                "part": {},
                "ng_quantity": false,
                "supplier": {},
                "is_urgent": false,
                "is_sampling": "全检",
                "id": 0,
                "quantity": false
            },
            "state": false,
            "quantity": false,
            "id": 0,
            "inspected_qty": 0
        },
        "id": 1
    },
    {
        "pos_z": 2,
        "pos_x": 1,
        "pos_y": 1,
        "name": "1-1-2",
        "state": "empty",
        "active": true,
        "package": {
            "qr_code": "",
            "batch": {
                "work_no": false,
                "inspection_quantity": false,
                "packaged_quantity": false,
                "order_no": false,
                "state": false,
                "ok_quantity": false,
                "pos": false,
                "inspection_datetime": null,
                "arrival_date_str": "",
                "part": {},
                "ng_quantity": false,
                "supplier": {},
                "is_urgent": false,
                "is_sampling": "全检",
                "id": 0,
                "quantity": false
            },
            "state": false,
            "quantity": false,
            "id": 0,
            "inspected_qty": 0
        },
        "id": 11
    },
    {
        "pos_z": 3,
        "pos_x": 1,
        "pos_y": 1,
        "name": "1-1-3",
        "state": "empty",
        "active": true,
        "package": {
            "qr_code": "",
            "batch": {
                "work_no": false,
                "inspection_quantity": false,
                "packaged_quantity": false,
                "order_no": false,
                "state": false,
                "ok_quantity": false,
                "pos": false,
                "inspection_datetime": null,
                "arrival_date_str": "",
                "part": {},
                "ng_quantity": false,
                "supplier": {},
                "is_urgent": false,
                "is_sampling": "全检",
                "id": 0,
                "quantity": false
            },
            "state": false,
            "quantity": false,
            "id": 0,
            "inspected_qty": 0
        },
        "id": 21
    },
    {
        "pos_z": 1,
        "pos_x": 1,
        "pos_y": 2,
        "name": "1-2-1",
        "state": "empty",
        "active": true,
        "package": {
            "qr_code": "",
            "batch": {
                "work_no": false,
                "inspection_quantity": false,
                "packaged_quantity": false,
                "order_no": false,
                "state": false,
                "ok_quantity": false,
                "pos": false,
                "inspection_datetime": null,
                "arrival_date_str": "",
                "part": {},
                "ng_quantity": false,
                "supplier": {},
                "is_urgent": false,
                "is_sampling": "全检",
                "id": 0,
                "quantity": false
            },
            "state": false,
            "quantity": false,
            "id": 0,
            "inspected_qty": 0
        },
        "id": 31
    },
    {
        "pos_z": 1,
        "pos_x": 2,
        "pos_y": 2,
        "name": "2-2-1",
        "state": "empty",
        "active": true,
        "package": {
            "qr_code": "",
            "batch": {
                "work_no": false,
                "inspection_quantity": false,
                "packaged_quantity": false,
                "order_no": false,
                "state": false,
                "ok_quantity": false,
                "pos": false,
                "inspection_datetime": null,
                "arrival_date_str": "",
                "part": {},
                "ng_quantity": false,
                "supplier": {},
                "is_urgent": false,
                "is_sampling": "全检",
                "id": 0,
                "quantity": false
            },
            "state": false,
            "quantity": false,
            "id": 0,
            "inspected_qty": 0
        },
        "id": 32
    },
    {
        "pos_z": 2,
        "pos_x": 2,
        "pos_y": 2,
        "name": "2-2-2",
        "state": "empty",
        "active": true,
        "package": {
            "qr_code": "",
            "batch": {
                "work_no": false,
                "inspection_quantity": false,
                "packaged_quantity": false,
                "order_no": false,
                "state": false,
                "ok_quantity": false,
                "pos": false,
                "inspection_datetime": null,
                "arrival_date_str": "",
                "part": {},
                "ng_quantity": false,
                "supplier": {},
                "is_urgent": false,
                "is_sampling": "全检",
                "id": 0,
                "quantity": false
            },
            "state": false,
            "quantity": false,
            "id": 0,
            "inspected_qty": 0
        },
        "id": 42
    },
    {
        "pos_z": 3,
        "pos_x": 2,
        "pos_y": 2,
        "name": "2-2-3",
        "state": "empty",
        "active": true,
        "package": {
            "qr_code": "",
            "batch": {
                "work_no": false,
                "inspection_quantity": false,
                "packaged_quantity": false,
                "order_no": false,
                "state": false,
                "ok_quantity": false,
                "pos": false,
                "inspection_datetime": null,
                "arrival_date_str": "",
                "part": {},
                "ng_quantity": false,
                "supplier": {},
                "is_urgent": false,
                "is_sampling": "全检",
                "id": 0,
                "quantity": false
            },
            "state": false,
            "quantity": false,
            "id": 0,
            "inspected_qty": 0
        },
        "id": 52
    },
    {
        "pos_z": 1,
        "pos_x": 3,
        "pos_y": 1,
        "name": "3-1-1",
        "state": "empty",
        "active": true,
        "package": {
            "qr_code": "",
            "batch": {
                "work_no": false,
                "inspection_quantity": false,
                "packaged_quantity": false,
                "order_no": false,
                "state": false,
                "ok_quantity": false,
                "pos": false,
                "inspection_datetime": null,
                "arrival_date_str": "",
                "part": {},
                "ng_quantity": false,
                "supplier": {},
                "is_urgent": false,
                "is_sampling": "全检",
                "id": 0,
                "quantity": false
            },
            "state": false,
            "quantity": false,
            "id": 0,
            "inspected_qty": 0
        },
        "id": 3
    },
    {
        "pos_z": 2,
        "pos_x": 3,
        "pos_y": 1,
        "name": "3-1-2",
        "state": "empty",
        "active": true,
        "package": {
            "qr_code": "",
            "batch": {
                "work_no": false,
                "inspection_quantity": false,
                "packaged_quantity": false,
                "order_no": false,
                "state": false,
                "ok_quantity": false,
                "pos": false,
                "inspection_datetime": null,
                "arrival_date_str": "",
                "part": {},
                "ng_quantity": false,
                "supplier": {},
                "is_urgent": false,
                "is_sampling": "全检",
                "id": 0,
                "quantity": false
            },
            "state": false,
            "quantity": false,
            "id": 0,
            "inspected_qty": 0
        },
        "id": 13
    },
    {
        "pos_z": 3,
        "pos_x": 3,
        "pos_y": 1,
        "name": "3-1-3",
        "state": "empty",
        "active": true,
        "package": {
            "qr_code": "",
            "batch": {
                "work_no": false,
                "inspection_quantity": false,
                "packaged_quantity": false,
                "order_no": false,
                "state": false,
                "ok_quantity": false,
                "pos": false,
                "inspection_datetime": null,
                "arrival_date_str": "",
                "part": {},
                "ng_quantity": false,
                "supplier": {},
                "is_urgent": false,
                "is_sampling": "全检",
                "id": 0,
                "quantity": false
            },
            "state": false,
            "quantity": false,
            "id": 0,
            "inspected_qty": 0
        },
        "id": 23
    },
    {
        "pos_z": 1,
        "pos_x": 3,
        "pos_y": 2,
        "name": "3-2-1",
        "state": "empty",
        "active": true,
        "package": {
            "qr_code": "",
            "batch": {
                "work_no": false,
                "inspection_quantity": false,
                "packaged_quantity": false,
                "order_no": false,
                "state": false,
                "ok_quantity": false,
                "pos": false,
                "inspection_datetime": null,
                "arrival_date_str": "",
                "part": {},
                "ng_quantity": false,
                "supplier": {},
                "is_urgent": false,
                "is_sampling": "全检",
                "id": 0,
                "quantity": false
            },
            "state": false,
            "quantity": false,
            "id": 0,
            "inspected_qty": 0
        },
        "id": 33
    },
    {
        "pos_z": 2,
        "pos_x": 3,
        "pos_y": 2,
        "name": "3-2-2",
        "state": "empty",
        "active": true,
        "package": {
            "qr_code": "",
            "batch": {
                "work_no": false,
                "inspection_quantity": false,
                "packaged_quantity": false,
                "order_no": false,
                "state": false,
                "ok_quantity": false,
                "pos": false,
                "inspection_datetime": null,
                "arrival_date_str": "",
                "part": {},
                "ng_quantity": false,
                "supplier": {},
                "is_urgent": false,
                "is_sampling": "全检",
                "id": 0,
                "quantity": false
            },
            "state": false,
            "quantity": false,
            "id": 0,
            "inspected_qty": 0
        },
        "id": 43
    },
    {
        "pos_z": 3,
        "pos_x": 3,
        "pos_y": 2,
        "name": "3-2-3",
        "state": "empty",
        "active": true,
        "package": {
            "qr_code": "",
            "batch": {
                "work_no": false,
                "inspection_quantity": false,
                "packaged_quantity": false,
                "order_no": false,
                "state": false,
                "ok_quantity": false,
                "pos": false,
                "inspection_datetime": null,
                "arrival_date_str": "",
                "part": {},
                "ng_quantity": false,
                "supplier": {},
                "is_urgent": false,
                "is_sampling": "全检",
                "id": 0,
                "quantity": false
            },
            "state": false,
            "quantity": false,
            "id": 0,
            "inspected_qty": 0
        },
        "id": 53
    },
    {
        "pos_z": 1,
        "pos_x": 4,
        "pos_y": 1,
        "name": "4-1-1",
        "state": "empty",
        "active": true,
        "package": {
            "qr_code": "",
            "batch": {
                "work_no": false,
                "inspection_quantity": false,
                "packaged_quantity": false,
                "order_no": false,
                "state": false,
                "ok_quantity": false,
                "pos": false,
                "inspection_datetime": null,
                "arrival_date_str": "",
                "part": {},
                "ng_quantity": false,
                "supplier": {},
                "is_urgent": false,
                "is_sampling": "全检",
                "id": 0,
                "quantity": false
            },
            "state": false,
            "quantity": false,
            "id": 0,
            "inspected_qty": 0
        },
        "id": 4
    }
]

```
