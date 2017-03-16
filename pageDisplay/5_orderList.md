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
| conId | 用户id  |string | 是 |
| sysAccount | 账套号 |string | 是 |
| pageNo | 页码，用于分页，默认值为1 |string |否|
| pageSize | 每页显示数，用于分页，默认值为10 |string |否|

### 请求参数示例

```json
{
    conId: "705FC5426B1B45F491509804B9DFCF16",
    sysAccount: "WKZZ",
    pageNo: "1",
    pageSize: "10"
}
```

### 返回参数

| 参数名称 |类型 |说明 |
| --------- | ------------ | ------ |
| orderId| string | 订单ID |
| orderNo| string | 订单编号 |
| status| num | 订单状态 |
| sum| num | 订单商品数 |
| totalPrice| num | 总价 |
| defaultPic| num | 订单默认商品图片 |
| defaultTitle| num | 订单默认商品名称 |
| defaultContent| num | 订单默认商品描述 |

### 返回示例
```json
{
    "result": [
        {
            "orderId":"",
            "orderNo":"",
            "status":"",
            "sum":"",
            "totalPrice":"",
            "defaultPic":"",
            "defaultTitle":"",
            "defaultContent":""
        },
        {
            "orderId":"",
            "orderNo":"",
            "status":"",
            "sum":"",
            "totalPrice":"",
            "defaultPic":"",
            "defaultTitle":"",
            "defaultContent":""
        },
        {
            "orderId":"",
            "orderNo":"",
            "status":"",
            "sum":"",
            "totalPrice":"",
            "defaultPic":"",
            "defaultTitle":"",
            "defaultContent":""
        }
    ],
    "resultCode": 1
}
```

###备注

需求中所列为前端必需字段，后台开发可根据开发需要新增或修改字段。








