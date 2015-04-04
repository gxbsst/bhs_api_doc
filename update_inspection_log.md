# 更新检测结果

### URL

`http://host/api/iqc/inspection_logs?database=<database>&access_token=<access_token>`

##### HTTP 方法:

PATCH

#####参数详细:

**database**: 当前openerp启动使用的数据名字, 请咨询API开发者。

**access_token**:  用户登陆token， 请咨询API开发者

**batch_id**: batch id

**package_id**: package id

**log_id"**: [提交检测结果](create_inspection_log.md) 返回的id

**measurement**: 如果该检测点为定量，则输入测量值

**description**: 如果有错误， 则为描述错误的内容

**status**: 如果为定性，则需要输入`ng` 或者 `ok`

**fail_code_id**: 错误代码id

**ng_qty**: 出现该错误的零件数

** 返回 **:

参考一下

``` json
{
"id": 1,
"status":"ng",
"description": "hhhh",
"order_no": "1",
"part_no": 1,
"pos": 1,
"package_id": 2,
"part_id": 1,
"measurement": 110.2,
"inspection_id": 9,
"batch_id": 3,
"inspector_id": 1,
"rule_id": 1,
"ng_qty": 1,
"fail_code_id": 1
}
```
