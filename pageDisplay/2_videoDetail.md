# 2.2 视频详情页

- [2.2.1 获取视频详情](#detail) 
- [2.2.2 获取评价详情](#comments)
- [2.2.3发送评论](#updatecomment)

## 2.2.1 获取视频详情 {#detail}

### 接口描述

获取视频详情，包括当前视频包名称、视频包信息以及视频包下所有视频信息

## 2.2.2 获取评价详情 {#comments}

### 接口描述

视频（包）详情页获取视频（包）评价

## 接口地址

> http://www.hubeta.com/web/api/product/qryReview

## 请求方式

> POST

## 请求参数

| 参数名称 |说明 |类型 |
| --------- | ------------ | ------ |
| productId | 产品包id  |string |
| sysAccount | 账套号 |string |
| pageNo | 页码，用于分页 |string |
| pageSize | 每页显示数，用于分页 |string |

## 请求参数示例

```json
{
    pntID:"id";
	conID:"id";
	pageSize
}
```

## 返回参数

| 参数名称 |类型 |说明 |
| --------- | ------------ | ------ |
| result | string |返回删除产品包操作成功 |



## 返回示例
```json
{
    "result": [
        [
            {
                "pntID": "id",
                "conID": "id",
                "headURL": "url",
                "name": "细节决定成败",
                "time": "2017/3/16",
                "conTent": "地球已经危在旦夕"
            }
        ],
        [
            {
                "pntID": "id",
                "conID": "id",
                "headURL": "url",
                "name": "细节决定成败",
                "time": "2017/3/16",
                "conTent": "地球已经危在旦夕"
            }
        ]
    ],
    "resultCode": 1
}
```

##备注

需求中所列为前端必需字段，后台开发可根据开发需要新增或修改字段。

## 2.2.3 发送评论 {#updatecomment}