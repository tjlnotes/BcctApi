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
| categoryName | 分类名称 |num |
| categoryId | 分类ID】 |num |
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

获取对应分类页页面信息，根据partType字段，即后台配置的区块显示的组件类型（组件类型：0.轮播；1.宫格；2.直排；3.滑块；4.选项卡】）返回组件信息，如轮播时返回资源链接地址，宫格时返回商品信息。

### 接口地址

> http://www.hubeta.com/web/api/page/getPage

### 请求方式

> POST

### 请求参数

| 参数名称 |说明 |类型 |是否必需|
| --------- | ------------ | ------ | ----- |
| sysAccount | 账套号 |string |是 |
| sysAccount | 账套号 |string |是 |

### 请求参数示例

```json
{
  sysAccount:'WKZZ',
  categoryId:''
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
  "result": [
    {
      "displaySeq": 1,
      "partType": 2,
      "needButton": 0,
      "detailList": [
        {
          "displaySeq": 1,
          "resourceId": "49A68186E5764E22E053F401A8C0704D",
          "hrefUrl": "http://www.hubeta.com/wechat-api/resources/WKZZ/html/activity/activity.html?sysAccount=WKZZ&ployId=9E7B20EF4D8C4ECB941804875FB3ECA1",
          "needButton": 0,
          "resourceUrl": "http://www.hubeta.com:8080/group1/M00/00/14/wKgB9Fi2bAKAWJ07AABPPREW8oY717.jpg",
          "linkType": 5,
          "resourceType": 0,
        },
        {
          "displaySeq": 2,
          "resourceId": "4876407E9DB443DCE053F401A8C0FDB0",
          "hrefUrl": "http://www.hubeta.com/wechat-api/resources/WKZZ/html/activity/activity.html?sysAccount=WKZZ&ployId=B2198CD7A9EF4C8783E7AED9BBE00A62",
          "needButton": 0,
          "resourceUrl": "http://www.hubeta.com:8080/group1/M00/00/11/wKgB9FiievKAValUAACzFWrIC5g161.jpg",
          "linkType": 5,
          "resourceType": 0
        },
      ]
    },
    {
      "displaySeq": 3,
      "partType": 2,
      "needButton": 0,
      "productInfo": {
        "displaySeq": 1,
        "salPrice": 1699,
        "pntStock": 13,
        "agent": 15,
        "productName": "Kimi英语",
        "content": "促进孩子说的欲望，丰富孩子的英语词汇量",
        "playAccount": "1550",
        "id": "705FC5426B1B45F491509804B9DFCF16",
        "productCode": "WVBQFS2023-2",
      }
    },
  ],
  "resultCode": 1
}
```

###备注

需求中所列为前端必需字段，后台开发可根据开发需要新增或修改字段。