# 看板

### URL

`http://host/api/iqc/kanban?database=<database>&access_token=<access_token>`

##### HTTP 方法:
GET

#####参数详细:

**database**: 当前openerp启动使用的数据名字, 请咨询API开发者。

**access_token**:  用户登陆token， 请咨询API开发者

** 返回 **:

参考一下

``` json

{
    't_packaged_quantity': 0,
    't_inspected_quantity': 0,
    't_ok_quantity': 0,
    't_ng_quantity': 0,

    't_stock_location_number': 0,
    'empty_location_number': 0,
    'full_location_number': 0,

    'cp_inspector_name': '',
    'cp_part_no': '',
    'cp_part_name': '',
    'cp_supplier_name': '',
    'cp_t_packaged_quantity': 0,
    'cp_packaged_quantity': 0,

    'ci_inspector_name_1': '',
    'ci_part_no_1': '',
    'ci_part_name_1': '',
    'ci_supplier_name_1': '',
    'ci_inspected_quantity_1': 0,
    'ci_not_inspected_quantity_1': 0,
    'ci_ok_quantity_1': 0,
    'ci_ng_quantity_1': 0,

    'ci_inspector_name_2': '',
    'ci_part_no_2': '',
    'ci_part_name_2': '',
    'ci_supplier_name_2': '',
    'ci_inspected_quantity_2': 0,
    'ci_not_inspected_quantity_2': 0,
    'ci_ok_quantity_2': 0,
    'ci_ng_quantity_2': 0,
}

```
