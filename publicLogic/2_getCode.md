# 2.2 获取验证码

## 接口描述

根据用户conId获取用户所有数据

### 接口地址

> http://www.hubeta.com/web/api/tldIdentifyCode/get

### 请求方式

> POST

### 请求参数

| 参数名称 |说明 |类型 |是否必需|
| --------- | ------------ | ------ | ----- |
| conId | 用户conId |string |是 |
| sysAccount| 账套号 |string |是 |
| mobile | 用户手机号 |string |是 |

### 请求参数示例

```json
{
    "conId":"DD0A1E6556DA4393A2D8EE09755C3110",
    "sysAccount":"WKZZ",
    "mobile":"13011202787"
}
```

### 返回参数

| 参数名称 |说明 |类型 |
| --------- | ------------ | ------ |
|resultCode| 接口返回码:1-成功，0-失败 | num |

### 返回示例

```json
{
    "resultCode": 1
}
```

###备注

需求中所列为前端必需字段，后台开发可根据开发需要新增或修改字段。
