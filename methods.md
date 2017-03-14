# 公共逻辑类接口

Methods allow you to smoothly display code examples in different languages.


## 1. 获取用户conid
#### 接口描述
    

My first method exposes how to print a message in JavaScript and Go.
#### 请求接口
>  

#### 请求方式
> POST

#### 请求参数

| 参数名称  |说明            |类型    |是否必需|
| --------- | ------------ | ------ | ----- |
| conId     | 用户信息conId |string  |是      |

#### 请求示例

```json
{
  conId: 'DD0A1E6556DA4393A2D8EE09755C3110'
}

```
#### 返回参数

| 参数名称  |说明            |类型    |是否必需|
| --------- | ------------ | ------ | ----- |
| city     | 用户信息conId |string  |是      |
| conName     | 用户信息conId |string  |是      |
| conNo     | 用户信息conId |string  |是      |
| conType     | 用户信息conId |string  |是      |
| country     | 用户信息conId |string  |是      |
| createBy     | 用户信息conId |string  |是      |
| createDt     | 用户信息conId |string  |是      |
| enabled     | 用户信息conId |string  |是      |
| eonQrcode     | 用户信息conId |string  |是      |
| firstId     | 用户信息conId |string  |是      |
| homePic     | 用户信息conId |string  |是      |
| id     | 用户信息conId |string  |是      |
| isLockout     | 用户信息conId |string  |是      |
| memo     | 用户信息conId |string  |是      |
| mobile     | 用户信息conId |string  |是      |
| pic     | 用户信息conId |string  |是      |
| province     | 用户信息conId |string  |是      |
| sex     | 用户信息conId |string  |是      |
| sourceId     | 用户信息conId |string  |是      |
| conId     | 用户信息conId |string  |是      |
| status     | 用户信息conId |string  |是      |
| subscribe     | 用户信息conId |string  |是      |
| subscribeDt     | 用户信息conId |string  |是      |
| sysAccount     | 用户信息conId |string  |是      |
| twitterCngDt     | 用户信息conId |string  |是      |
| twitterDt     | 用户信息conId |string  |是      |
| twitterOrder     | 用户信息conId |string  |是      |
| updateDt     | 用户信息conId |string  |是      |
| userId     | 用户信息conId |string  |是      |
| twitterOrder     | 用户信息conId |string  |是      |

#### 返回示例

```json
{
  "result": {
    "city": "长沙市",
    "conName": "张三",
    "conNo": 1,
    "conType": 1,
    "country": "中国",
    "createBy": "system",
    "createDt": "2016-12-26 14:18:48",
    "enabled": 1,
    "eonQrcode": 0,
    "firstId": "0",
    "homePic": "http://www.hubeta.com:8080/group1/M00/00/12/wKgB9FiruwyAY2qBAAaFB42OxaI144.jpg",
    "id": "DD0A1E6556DA4393A2D8EE09755C3110",
    "isLockout": 0,
    "memo": "971731",
    "mobile": "18588474441",
    "pic": "http://www.hubeta.com:8080/group1/M00/00/07/wKgB9FhgtkiAAEe2AAAFJgnHYyM520.jpg",
    "province": "湖南省",
    "sex": 1,
    "sourceId": "o2HCxwXblItq9f_-4ss3cHfRSyvE",
    "status": 0,
    "subscribe": 1,
    "subscribeDt": "2016-12-26 14:18:48",
    "sysAccount": "WKZZ",
    "twitterCngDt": "2017-01-03 09:40:52",
    "twitterDt": "2017-01-03 09:40:52",
    "twitterOrder": "EBF87AE519B548B0B630615E1CE626C1",
    "updateDt": "2017-01-03 09:38:04",
    "userId": "5DDA29C3694D478A8930198BB56C6760",
    "version": 1
  },
  "resultCode": 1
}
```
