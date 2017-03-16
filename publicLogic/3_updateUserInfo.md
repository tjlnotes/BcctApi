# 1.3 修改用户信息

### 接口描述

根据用户ID和套账号修改用户信息

### 接口地址

> http://www.hubeta.com/web/api/basCustomer/updateCustomer

### 请求方式

> POST

### 请求参数

| 参数名称 | 说明 | 类型 | 是否必需 |
| --- | --- | --- | --- |
| conId | 用户ID | string | 是 |
| sysAccount |账套号| string|是|
|mobile|手机号|num|否|
|name|用户昵称|string|否|

### 请求参数示例

```json
{
  "sysAccount":'WKZZ',
  "conId":"AHIWUR7127846HHA",
  "mobile":"13311222787"
}
```

### 返回参数

| 参数名称 | 说明 | 类型 |
| :--- | :--- | :--- |
| resultCode | 请求参数码，1成功，0失败 | num |

### 返回示例

```json
{
  "resultCode": 1
}
```

### 备注

用户ID和账套号为必需参数，其余为可选得更新参数，此处只列举了手机号和昵称，按情况添加。

