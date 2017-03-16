# 首页

## 获取页面分类接口

### 接口描述

获取页面分类类名

### 接口地址

> http://www.hubeta.com/web/api/pntProduct/getPntCategories

### 请求方式

> POST

### 请求参数

| 参数名称 |说明 |类型 |是否必需|
| --------- | ------------ | ------ | ----- |
| sysAccount| 账套号 |string |是 |

### 请求参数示例

```json
{
  sysAccount:'WKZZ'
}
```

### 返回参数

| 参数名称 |说明 |类型 |
| --------- | ------------ | ------ |
| displaySeq | 显示序号 |num|
| categoryName | 会员代码【可自定义编码规则】 |num |
| resultCode | 请求参数码，1成功，0失败 |num |

### 返回示例

```json
{
  "result": [
    {
      "displaySeq": 1,
      "categoryName": "枕芯类"
    },
    {
      "displaySeq": 2,
      "categoryName": "套件类"
    },
    {
      "displaySeq": 3,
      "categoryName": "被芯类",
    },
    {
      "displaySeq": 4,
      "categoryName": "家居小件",
    }
  ],
  "resultCode": 1
}
```

###备注

需求中所列为前端必需字段，后台开发可根据开发需要新增或修改字段。

## 获得分类页面信息接口

### 接口描述

获取对应分类页页面信息

### 接口地址

> http://www.hubeta.com/web/api/page/getPage

### 请求方式

> POST

### 请求参数

| 参数名称 |说明 |类型 |是否必需|
| --------- | ------------ | ------ | ----- |
| conId | 用户信息conId |string |是 |
| conId | 用户信息conId |string |是 |
| conId | 用户信息conId |string |是 |

### 请求参数示例

```json
{
conId:'DD0A1E6556DA4393A2D8EE09755C3110'
}
```

### 返回参数

| 参数名称 |说明 |类型 |
| --------- | ------------ | ------ |
| id | 会员编号 |string |
| conName | 用户名 |string |
| conNo | 会员代码【可自定义编码规则】 |num |
| conType | 会员类型 0普通客户 1代理客户【推客】 |num |
| country | 国家 |string |
| province | 省份 |string |
| city | 城市 |string |
| mobile | 手机号 |string |
| pic | 头像图片 |string |
| sex | 用户信息conId |string |
| resultCode | 查询结果，取值为0和1 ，0表示查询失败，1表示查询成功|num
| sysAccount | 账套号 | string

### 返回示例

```json
{
"result": {
"city": "长沙市",
"conName": "张三",
"conNo": 1,
"conType": 1,
"country": "中国",
"homePic": "http://www.hubeta.com:8080/group1/M00/00/12/wKgB9FiruwyAY2qBAAaFB42OxaI144.jpg",
"id": "DD0A1E6556DA4393A2D8EE09755C3110",
"memo": "971731",
"mobile": "18588474441",
"pic": "http://www.hubeta.com:8080/group1/M00/00/07/wKgB9FhgtkiAAEe2AAAFJgnHYyM520.jpg",
"province": "湖南省",
"sex": 1,
"sysAccount": "WKZZ"
},
"resultCode": 1
}
```

###备注

需求中所列为前端必需字段，后台开发可根据开发需要新增或修改字段。