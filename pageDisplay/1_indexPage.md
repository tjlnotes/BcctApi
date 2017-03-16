# 2.1 首页

* [2.1.1获取页面分类接口](#2.1.1)
* [2.1.2获取分类页面信息接口](#2.1.2)

## 2.1.1获取页面分类接口  {#2.1.1}

### 接口描述

获取页面分类类名

### 接口地址

> [http://www.hubeta.com/web/api/pntProduct/getPntCategories](http://www.hubeta.com/web/api/pntProduct/getPntCategories)

### 请求方式

> POST

### 请求参数

| 参数名称 | 说明 | 类型 | 是否必需 |
| --- | --- | --- | --- |
| sysAccount | 账套号 | string | 是 |

### 请求参数示例

```json
{
  sysAccount:'WKZZ'
}
```

### 返回参数

| 参数名称 | 说明 | 类型 |
| :--- | :--- | :--- |
| displaySeq | 显示序号 | num |
| categoryName | 分类名称 | num |
| categoryCode | 分类代码 | num |
| resultCode | 请求参数码，1成功，0失败 | num |

### 返回示例

```json
{
  "result": [
    {
      "displaySeq": 1,
      "categoryCode": "01",
      "categoryName": "枕芯类"
    },
    {
      "displaySeq": 2,
      "categoryCode": "02",
      "categoryName": "套件类"
    },
    {
      "displaySeq": 3,
      "categoryCode": "03",
      "categoryName": "被芯类",
    },
    {
      "displaySeq": 4,
      "categoryCode": "04",
      "categoryName": "家居小件",
    }
  ],
  "resultCode": 1
}
```

### 备注

需求中所列为前端必需字段，后台开发可根据开发需要新增或修改字段。

## 2.1.2 获取分类页面信息接口  {#2.1.2}

### 接口描述

获取对应分类页页面信息，根据partType字段，即后台配置的区块显示的组件类型（组件类型：0.轮播，1.宫格，2.直排，3.滑块，4.选项卡】）返回组件信息，如轮播时返回资源链接地址，宫格时返回商品信息。

### 接口地址

> [http://www.hubeta.com/web/api/page/getPage](http://www.hubeta.com/web/api/page/getPage)

### 请求方式

> POST

### 请求参数

| 参数名称 | 说明 | 类型 | 是否必需 |
| --- | --- | --- | --- |
| sysAccount | 账套号 | string | 是 |
| categoryCode | 分类代码 | string | 是 |

### 请求参数示例

```json
{
  sysAccount:'WKZZ',
  categoryCode:'02'
}
```

### 返回参数

| 参数名称 | 说明 | 类型 |
| --- | --- | --- |
| displaySeq | 组件序列号 | num |
| partType | 组件类型：【0：轮播，1：宫格，2：直排，3：滑块，4：选项卡】 | num |
| needButton | 是否需要按钮： 【0：不需要，1：需要】 | num |
| resourceId | 资源ID | string |
| hrefUrl | 链接地址 | string |
| resourceUrl | 资源地址 | string |
| linkType | 链接类型【0：无链接；1：链接到产品；2：链接到分类；3:链接到 SKU；4：外部链接 5:链接到秒杀活动页】 | num |
| resourceType | 冗余字段：【0：图片；1：音频；2：视频；3：文本】 | string |
| salPrice | 售价 | num |
| agent | 折扣 | num |
| productName | 商品名称 | string |
| content | 商品描述 | string |
| playAccount | 播放次数 | num |
| productId | 商品ID | string |
| resultCode | 返回码 | num |

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
        "agent": 15,
        "productName": "Kimi英语",
        "content": "促进孩子说的欲望，丰富孩子的英语词汇量",
        "playAccount": "1550",
        "productId": "705FC5426B1B45F491509804B9DFCF16",
        "productCode": "WVBQFS2023-2",
      }
    },
  ],
  "resultCode": 1
}
```

### 备注

需求中所列为前端必需字段，后台开发可根据开发需要新增或修改字段。

