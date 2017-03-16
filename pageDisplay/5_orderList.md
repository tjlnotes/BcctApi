# 2.5 订单结算页

- [2.5.1 获取订单信息](#detail) 

## 2.5.1 获取订单列表信息 {#detail}

### 接口描述

获取当前用户是所有订单

### 接口地址

> http://www.hubeta.com/web/api/order/getList

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








