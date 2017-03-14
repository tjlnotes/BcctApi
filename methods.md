# 公共逻辑类接口

Methods allow you to smoothly display code examples in different languages.


## 1. 获取用户conid
#### 接口描述
    

My first method exposes how to print a message in JavaScript and Go.
#### 请求接口
>  

####请求示例

```
  
``` 

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

{% sample lang="go" %}
Here is how to print a message to `stdout` using Go.

```go
fmt.Println("My first method")
```

{% common %}
Whatever language you are using, the result will be the same.

```bash
$ My first method
```
{% endmethod %}
