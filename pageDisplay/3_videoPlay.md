# 2.3 视频播放页

- [2.3.1 获取视频详情](#detail) 

## 2.3.1 获取视频详情 {#detail}

### 接口描述

视频点播页，根据当前视频ID查询得到当前视频地址、图片、当前视频在视频包中所处集数、同视频包下其它视频ID、集数、名称、简介。

### 接口地址

> http://www.hubeta.com/wechat-api/wechat/getVideos

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
       "curUrl":
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
                       "time": "12分钟"
                   },
                   {
                       "title": "Unit02 数字世界",
                       "time": "12分钟"
                   }
               ]
           },
           {
               "theme": "主题二 快乐一家人",
               "content": [
                   {
                       "title": "Unit01 字母世界",
                       "time": "12分钟"
                   },
                   {
                       "title": "Unit02 数字世界",
                       "time": "12分钟"
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