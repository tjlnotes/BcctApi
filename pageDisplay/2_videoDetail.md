# 2.2 视频详情页

- [2.2.1 获取视频详情](#detail) 
- [2.2.2 获取评价详情](#comments)
- [2.2.3发送评论](#updatecomment)

## 2.2.1 获取视频详情 {#detail}

### 接口描述

获取视频详情，包括当前视频包名称、视频包信息以及视频包下所有视频信息

### 接口地址

> http://www.hubeta.com/wechat-api/wechat/qyrProductDetail

### 请求方式

> POST

### 请求参数

| 参数名称 | 说明 | 类型 | 是否必须 |
| --------- | ------------ | ------ | ----- |
| productId | 产品包id |string | 是 |
| sysAccount | 账套号 |string | 是 |

### 请求参数示例

```json
{
    "productId": "705FC5426B1B45F491509804B9DFCF16",
    "sysAccount": "WKZZ",
}
```

### 返回参数

| 参数名称 |类型 |说明 |
| --------- | ------------ | ------ |
| packageTitle | string | 视频包名称 |
| content| string | 视频包详情介绍 |
| price| num| 原价 |
| discountPrice| num| 折扣价 |
| theme| string | 主题 |
| title| string | 分集标题 |
| time| string | 时间 |
| resultCode| num | 返回码 |

### 返回示例
```json
{
  "result": {
       "packageTitle":"乐学包",
       "content": "“海洋世界系列”是《蓝猫淘气三千问》继“幽默系列”之后推出的又一历险类故事系列",
       "price": 118,
       "discountPrice": 69,
       "summary": [
           {
               "theme": "主题一 字母世界",
               "content": [
                   {
                       "title": "Unit01 字母世界",
                       "time": "12分钟",
                       "id": "H3GI18A7EYRGD",
                       "url": ""
                   },
                   {
                       "title": "Unit02 数字世界",
                       "time": "12分钟",
                       "id": "A72GD73GR7Y",
                       "url": ""
                   }
               ]
           },
           {
               "theme": "主题二 快乐一家人",
               "content": [
                   {
                       "title": "Unit01 字母世界",
                       "time": "12分钟",
                       "id": "A72GD73GR7Y",
                       "url": ""
                   },
                   {
                       "title": "Unit02 数字世界",
                       "time": "12分钟",
                       "id": "A72GD73GR7Y",
                       "url": ""
                   }
               ]
           }
       ]
  },
  "resultCode": 1
}
```

###备注

需求中所列为前端必需字段，后台开发可根据开发需要新增或修改字段。

## 2.2.2 获取评价详情 {#comments}

### 接口描述

视频（包）详情页获取视频（包）评价

### 接口地址

> http://www.hubeta.com/web/api/product/addReview

### 请求方式

> POST

### 请求参数

| 参数名称 | 说明 | 类型 | 是否必须 |
| --------- | ------------ | ------ | ----- |
| productId | 产品包id  |string | 是 |
| sysAccount | 账套号 |string | 是 |
| pageNo | 页码，用于分页，默认值为1 |string |否|
| pageSize | 每页显示数，用于分页，默认值为10 |string |否|

### 请求参数示例

```json
{
    productId: "705FC5426B1B45F491509804B9DFCF16",
    sysAccount: "WKZZ",
    pageNo: "1",
    pageSize: "10"
}
```

### 返回参数

| 参数名称 |类型 |说明 |
| --------- | ------------ | ------ |
| userName | string | 评论用户昵称 |
| userImage | string | 评论用户头像 |
| creatTime | string | 评论时间 |
| content | string | 评论内容 |
| resultCode | num | 返回码 |

### 返回示例
```json
{
    "result": [
        [
            {
                "userName": "张三",
                "userImage": "http://www.hubeta.com:8080/group1/M00/00/07/wKgB9FhgtkiAAEe2AAAFJgnHYyM520.jpg",
                "creatTime": "2017-03-15 10:23:58",
                "content": "地球已经危在旦夕地球已经危在旦夕"
            }
        ],
        [
            {
               "userName": "李四",
                "userImage": "http://www.hubeta.com:8080/group1/M00/00/07/wKgB9FhgtkiAAEe2AAAFJgnHYyM520.jpg",
                "creatTime": "2017-03-15 10:23:58",
                "content": "恐龙大量灭亡"
            }
        ]
    ],
    "resultCode": 1
}
```

###备注

需求中所列为前端必需字段，后台开发可根据开发需要新增或修改字段。

## 2.2.3 发送评论 {#updatecomment}

### 接口描述

用户发表评论接口

### 接口地址

> http://www.hubeta.com/web/api/product/addReview

### 请求方式

> POST

### 请求参数

| 参数名称 | 说明 | 类型 | 是否必须 |
| --------- | ------------ | ------ | ----- |
| productId | 产品包id  |string | 是 |
| sysAccount | 账套号 |string | 是 |
| userId | 评论用户ID |string |否|
| comment | 评论详情 |string |否|

### 请求参数示例

```json
{
    productId: "705FC5426B1B45F491509804B9DFCF16",
    sysAccount: "WKZZ",
    userId: "HA7W8ER09804B9DFCF16",
    comment: "请好好写接口"
}
```

### 返回参数

| 参数名称 |类型 |说明 |
| --------- | ------------ | ------ |
| resultCode | num | 返回码 |

### 返回示例
```json
{
    "resultCode": 1
}
```

###备注

需求中所列为前端必需字段，后台开发可根据开发需要新增或修改字段。

