#


# 获取某个零件检测图


### 描述
```
获取检测流程
```

### URL

`http://host/api/iqc/part_instruction_images/<part_id>/?database=<database>&access_token=<access_token>`

##### HTTP 方法:
GET

#####参数详细:

**database**: 当前openerp启动使用的数据名字, 请咨询API开发者。

**access_token**:  用户登陆token， 请咨询API开发者

**part_id**: 零件id

** 返回 **:

图片

