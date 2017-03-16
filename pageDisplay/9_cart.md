# 2.9 购物车页

- [2.9.1 获取购物车信息](#detail) 
- [2.9.2 修改购物车信息](#update)

## 2.9.1 获取购物车信息 {#detail}

### 接口描述

获取当前用户是所有订单

### 接口地址

> http://www.hubeta.com/web/api/cart/get

### 请求方式

> POST

### 请求参数

| 参数名称 | 说明 | 类型 | 是否必须 |
| --------- | ------------ | ------ | ----- |
| conId | 用户id  |string | 是 |

### 请求参数示例

```json
{
    conId: "DD0A1E6556DA4393A2D8EE09755C3110"
}
```

### 返回参数

| 参数名称 |类型 |说明 |
| --------- | ------------ | ------ |
| title| string | 商品名称 |
| content| string | 商品描述 |
| price| num | 原价 |
| discountPrice| num | 折扣价 |
| pic| string| 图片地址 |

### 返回示例
```json
{
    "result": [
        {
            "title":"",
            "content":""
            "price":"",
            "discountPrice":"",
            "pic":""
        },
        {
            "title":"",
            "content":""
            "price":"",
            "discountPrice":"",
            "pic":""
        },
        {
            "title":"",
            "content":""
            "price":"",
            "discountPrice":"",
            "pic":""
        },
    ],
    "resultCode": 1
}
```

###备注

需求中所列为前端必需字段，后台开发可根据开发需要新增或修改字段。

## 2.9.2 新增购物车信息 {#update}

### 接口描述

获取当前用户是所有订单

### 接口地址

> http://www.hubeta.com/web/api/cart/add

### 请求方式

> POST

### 请求参数

| 参数名称 | 说明 | 类型 | 是否必须 |
| --------- | ------------ | ------ | ----- |
| conId | 用户id  |string | 是 |
| productId | 用户id  |string | 是 |
| sysAccount | 用户id  |string | 是 |


### 请求参数示例

```json
{
    conId: "DD0A1E6556DA4393A2D8EE09755C3110"
}
```

### 返回参数

| 参数名称 |类型 |说明 |
| --------- | ------------ | ------ |
| title| string | 商品名称 |
| content| string | 商品描述 |
| price| num | 原价 |
| discountPrice| num | 折扣价 |
| pic| string| 图片地址 |

### 返回示例
```json
{
    "result": [
        {
            "title":"",
            "content":""
            "price":"",
            "discountPrice":"",
            "pic":""
        },
        {
            "title":"",
            "content":""
            "price":"",
            "discountPrice":"",
            "pic":""
        },
        {
            "title":"",
            "content":""
            "price":"",
            "discountPrice":"",
            "pic":""
        },
    ],
    "resultCode": 1
}
```

###备注

需求中所列为前端必需字段，后台开发可根据开发需要新增或修改字段。




