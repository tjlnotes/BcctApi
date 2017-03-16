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
| videoUrl| string | 视频地址 |
| videoImg| string | 视频包详情介绍 |
| videoNo| num| 原价 |
| discountPrice| num| 折扣价 |
| theme| string | 主题 |
| title| string | 分集标题 |
| time| string | 时间 |
| resultCode| num | 返回码 |

### 返回示例
```json
{
  "result": {
       "videoUrl": "http://www.hubeta.com:8080/group1/M00/00/15/wKgB9Fi2eOGAeI_sAABZcDjy19Y660.mp4",
       "videoImg": "http://www.hubeta.com:8080/wKgB9Fi2eOGAeI_sAABZcDjy19Y660.jpg",
       "videoContent": "蓝猫一行人来到了外星人的飞船..."
       "videoNo":"1"
       "similarVideo": [
           {
               "videoUrl": "http://www.hubeta.com:8080/group1/M00/00/15/wKgB9Fi2eOGAeI_sAABZcDjy19Y660.mp4",
               "videoImg": "http://www.hubeta.com:8080/wKgB9Fi2eOGAeI_sAABZcDjy19Y660.jpg",
               "videoContent": "外星人...",
               "videoNo":"2"

           },
           {
               "videoUrl": "http://www.hubeta.com:8080/group1/M00/00/15/wKgB9Fi2eOGAeI_sAABZcDjy19Y660.mp4",
                "videoImg": "http://www.hubeta.com:8080/wKgB9Fi2eOGAeI_sAABZcDjy19Y660.jpg",
                "videoContent": "蓝猫...",
                "videoNo":"2"
           }
       ]
  },
  "resultCode": 1
}
```

###备注

需求中所列为前端必需字段，后台开发可根据开发需要新增或修改字段。