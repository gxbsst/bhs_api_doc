# 检测某个零件的某部分

# 获取某个package

### URL

`http://host/api/iqc/packages/<qr_code>/?database=<database>&token=<access_token>`

##### HTTP 方法:
POST

#####参数详细:

**database**: 当前openerp启动使用的数据名字, 请咨询API开发者。

**access_token**:  用户登陆token， 请咨询API开发者

batch_id: 批次id,
package_id: package_id,
measurement: 如果为定量， 输入检测度量值(float)
description: 如果为ng，输入错误描述
status: 如果该步骤为定性，输入ng 或者 ok

** 返回 **:

```
{
  "status": "ng",
  "description": "hhhh",
  "order_no": "1",
  "part_no": "1",
  "pos": "1",
  "package_id": 2,
  "part_id": 1,
  "measurement": 110.2,
  "inspection_id": 9,
  "batch_id": 3,
  "inspector_id": 1,
  "rule_id": 1
}
``
