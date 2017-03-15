# 公共逻辑类接口

Methods allow you to smoothly display code examples in different languages.


## 1. 获取用户conid
#### 接口描述
    

My first method exposes how to print a message in JavaScript and Go.
#### 请求接口
>  http://www.hubeta.com/web/api/basCustomer/getByConId

#### 请求方式
> POST

#### 请求参数

| 参数名称  |说明            |类型    |是否必需|
| --------- | ------------ | ------ | ----- |
| conId     | 用户信息conId |string  |是      |

#### 请求示例

```json
{
  conId:'DD0A1E6556DA4393A2D8EE09755C3110'
}

```
#### 返回参数

| 参数名称  |说明            |类型    |
| --------- | ------------ | ------ |
| id | 会员编号 |string |
| conName     | 用户名 |string  |
| conNo     | 会员代码【可自定义编码规则】 |num  |
| conType     | 会员类型 0普通客户 1代理客户【推客】 |num  |
| country     | 国家 |string  |
| province    | 省份   |string |
| city | 城市 |string |
| mobile     | 手机号 |string  |
| pic     | 头像图片 |string  |
| sex     | 用户信息conId |string  |
| resultCode | 查询结果，取值为0和1 ，0表示查询失败，1表示查询成功|num


#### 返回示例

```json
{
  "result": {
    "city": "长沙市",
    "conName": "张三",
    "conNo": 1,
    "conType": 1,
    "country": "中国",
    "homePic": "http://www.hubeta.com:8080/group1/M00/00/12/wKgB9FiruwyAY2qBAAaFB42OxaI144.jpg",
    "id": "DD0A1E6556DA4393A2D8EE09755C3110",
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
