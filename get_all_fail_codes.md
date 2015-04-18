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

`update_at: 2015-4-18`
``` json

[
    {
        "fail_code_items": [
            {
                "id": 2,
                "description_en": "美国描述",
                "description": "中文描述"
            }
        ],
        "name_en": "Size deviation A(With Clear tolerance on drawing)",
        "code": 1,
        "id": 1,
        "name": "带公差尺寸偏差"
    },
    {
        "fail_code_items": [],
        "name_en": "Size deviation B(according to general tolerance)",
        "code": 1,
        "id": 2,
        "name": "未注公差尺寸偏差"
    },
    {
        "fail_code_items": [],
        "name_en": "Welding defect",
        "code": 3,
        "id": 3,
        "name": "焊接缺陷"
    },
    {
        "fail_code_items": [],
        "name_en": "Welding defect",
        "code": 4,
        "id": 4,
        "name": "外观缺陷"
    },
    {
        "fail_code_items": [],
        "name_en": "Special character defect",
        "code": 5,
        "id": 5,
        "name": "特殊特性不符"
    },
    {
        "fail_code_items": [],
        "name_en": "Thread Hole",
        "code": 6,
        "id": 6,
        "name": "螺纹孔精度"
    },
    {
        "fail_code_items": [],
        "name_en": "Missing machining / Missing spare parts",
        "code": 7,
        "id": 7,
        "name": "漏加工/ 漏配件"
    },
    {
        "fail_code_items": [],
        "name_en": "Wrong part delivered",
        "code": 8,
        "id": 8,
        "name": "零件送错"
    },
    {
        "fail_code_items": [],
        "name_en": "Quality file issue",
        "code": 9,
        "id": 9,
        "name": "提交文件不完整"
    },
    {
        "fail_code_items": [],
        "name_en": "Others",
        "code": 10,
        "id": 10,
        "name": "其他"
    },
    {
        "fail_code_items": [
            {
                "id": 1,
                "description_en": "11111",
                "description": "1111"
            }
        ],
        "name_en": "英文",
        "code": 111,
        "id": 11,
        "name": "中午"
    }
]

```
