# 提交检测结果


### 描述
```
将实际检测结果发送给MES
```

### URL

`http://host/api/iqc/inspection_logs?database=<database>&access_token=<access_token>`

##### HTTP 方法:

POST

#####参数详细:

**database**: 当前openerp启动使用的数据名字, 请咨询API开发者。

**access_token**:  用户登陆token， 请咨询API开发者

**batch_id**: batch id

**package_id**: package id

**measurement**: 如果该检测点为定量，则输入测量值(float)

**description**: 如果有错误(`ng`)， 则为描述错误的内容

**status**: 如果为定性，则需要输入`ng` 或者 `ok`

**fail_code_id**: 错误代码id

**ng_qty**: 出现该错误的零件数



** 返回 **:

参考一下

``` json

    {
        "status": "ng",
        "ng_qty": "",
        "description": "",
        "order_no": "0134799",
        "part_no": "10002",
        "fail_code_name": "",
        "fail_code_id": "",
        "pos": "001",
        "rule": {
            "reference_value": "",
            "tool": "工具1",
            "standard": 11,
            "down": 10,
            "step": 1,
            "part_id": 13,
            "id": 1,
            "unit": "mm",
            "name": "步骤1",
            "coord_y": 21,
            "coord_x": 11,
            "standard_str": "",
            "up": 15,
            "type": "quantitative"
        },
        "fail_code_description": "",
        "package_id": "",
        "inspection_id": 3,
        "fail_code_code": "",
        "part_id": 13,
        "measurement": 1,
        "batch_id": 12,
        "inspector_id": 24,
        "id": 2,
        "ncr_id": 3
    }
```
