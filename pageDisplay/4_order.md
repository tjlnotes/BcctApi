# 2.4 订单结算页

- [2.4.1 获取订单信息](#detail) 
- [2.4.2 订单支付](#pay)
- [2.4.3 取消订单](#cancel)

## 2.4.1 获取订单信息 {#detail}

### 接口描述

获取订单信息

### 接口地址

> http://www.hubeta.com/web/api/cart/getById

### 请求方式

> POST

### 请求参数

| 参数名称 | 说明 | 类型 | 是否必需 |
| --- | --- | --- | --- |
| orderId | 订单编号 | string | 是 |
| sysAccount | 账套号 | string | 是 |

### 请求参数示例

```json
{
  "orderId":"ADFH91435H9AE9234",
  "sysAccount":"WKZZ"
}
```

### 返回参数

| 参数名称 | 说明 | 类型 |
| :--- | :--- | :--- |
| title| 视频包名称 | string |
| picUrl| 视频包图片 | string|
| content| 视频包简介 | string |
| price| 视频包单价 | num |
| totalPrice| 总价 | num |
| discountPrice| 优惠金额 | num |
| resultCode | 请求参数码，1成功，0失败 | num |

### 返回示例

```json
{
  "productList": [
    {
      "title": "英语包",
      "picUrl": "01",
      "content": "这是个英语包",
      "price":"12"
    },
    {
      "title": "趣味包",
      "picUrl": "http://123.52.242.20/pic/1.jpg",
      "content": "这是个趣味包",
      "price":"12"
    }
  ],
  "totalPrice":"24",
  "discountPrice":"20",
  "resultCode": 1
}
```

### 备注

需求中所列为前端必需字段，后台开发可根据开发需要新增或修改字段。


## 2.4.2 订单支付 {#pay}

### 接口描述

发起支付

### 接口地址

> http://www.hubeta.com/wechat-api/wechat/pay/createBill

### 请求方式

> POST

### 请求参数

| 参数名称 | 说明 | 类型 | 是否必需 |
| --- | --- | --- | --- |
| orderId | 订单编号 | string | 是 |
| fee | 支付费用 | num | 是 |
| sysAccount | 账套号 | string | 是 |

### 请求参数示例

```json
{
  "orderId":"ADFH91435H9AE9234",
  "fee":"20",
  "sysAccount":"WKZZ"
}
```

### 返回参数

| 参数名称 | 说明 | 类型 |
| :--- | :--- | :--- |
| appId| 发起微信支付字段 | string |
| nonceStr| 发起微信支付字段  | string|
| package| 发起微信支付字段  | string |
| paySign| 发起微信支付字段  | string|
| signType| 发起微信支付字段  | string|
| timeStamp| 发起微信支付字段  | string|
| resultCode | 请求参数码，1成功，0失败 | num |

### 返回示例

```json
{
  "result": {
    "appId": "wx7f19ea8d36f01072",
    "nonceStr": "2u5osfiqy2fclnr5pax7b12brlea8g3e",
    "package": "prepay_id=wx20170316225955551e9990930561892842",
    "paySign": "079CDCB12675166D9FBAEDBEAEF6D46E",
    "signType": "MD5",
    "timeStamp": "1489676395"
  },
  "resultCode": 1
}
```

### 备注

需求中所列为前端必需字段，后台开发可根据开发需要新增或修改字段。

## 2.4.2 取消订单 {#cancel}







