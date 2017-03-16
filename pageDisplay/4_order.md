# 2.4 订单结算页

- [2.4.1 获取订单信息](#detail) 
- [2.4.2 订单支付](#pay)
- [2.4.3 取消订单](#cancel)

## 2.4.1 获取订单信息 {#detail}

### 接口描述

获取订单信息

### 接口地址

> http://www.hubeta.com/web/api/pntProduct/getPntCategories

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


## 2.4.2 订单支付 {#pay}

## 2.4.2 取消订单 {#cancel}







