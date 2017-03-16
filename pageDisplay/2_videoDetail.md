- 购买页api

**请求URL：** 
- ` /*http://xx.com/api/user/register */`
  
**请求方式：**
- POST 


 **请求示例：** 
- ` /*http://xx.com//wechat/qyrProductDetail?username=JZJ&&password=123456&&name=zzh */`

 **返回示例**

```
{
"result":{
    "videoimg": "url",
    "video": "url",
    "details": {
        "title": "标题",
        "content": "海洋系列 是继...",
        "price": "68",
        "discount": "118",
        "crowd": "适合人群"
    },
    "productcontent": {
        "videolength": "30",
        "timelength": "150",
        "titletheme": {
            "list": [
                [
                    "Unit01",
                    "字母世界",
                    "12"
                ],
                [
                    "Unit02",
                    "字母世界",
                    "12"
                ],
                [
                    "Unit03",
                    "字母世界",
                    "12"
                ]
            ],
            "list": [
                [
                    "Unit01",
                    "字母世界",
                    "12"
                ],
                [
                    "Unit02",
                    "字母世界",
                    "12"
                ],
                [
                    "Unit03",
                    "字母世界",
                    "12"
                ]
            ],
            "list": [
                [
                    "Unit01",
                    "字母世界",
                    "12"
                ],
                [
                    "Unit02",
                    "字母世界",
                    "12"
                ],
                [
                    "Unit03",
                    "字母世界",
                    "12"
                ]
            ],
            "themecount": "一",
            "themetile": "字母世界"
        }
    },
    "comment": [
        {
            "head": "URL",
            "name": "细节决定成败",
            "postedtime": "2017/3/15",
            "commentcontent": "地球已经危在旦夕..."
        },
        {
            "head": "URL",
            "name": "细节决定成败",
            "postedtime": "2017/3/15",
            "commentcontent": "地球已经危在旦夕..."
        },
        {
            "head": "URL",
            "name": "细节决定成败",
            "postedtime": "2017/3/15",
            "commentcontent": "地球已经危在旦夕..."
        },
        {
            "head": "URL",
            "name": "细节决定成败",
            "postedtime": "2017/3/15",
            "commentcontent": "地球已经危在旦夕..."
        },
        {
            "head": "URL",
            "name": "细节决定成败",
            "postedtime": "2017/3/15",
            "commentcontent": "地球已经危在旦夕..."
        },
        {
            "head": "URL",
            "name": "细节决定成败",
            "postedtime": "2017/3/15",
            "commentcontent": "地球已经危在旦夕..."
        },
        {
            "head": "URL",
            "name": "细节决定成败",
            "postedtime": "2017/3/15",
            "commentcontent": "地球已经危在旦夕..."
        },
        {
            "head": "URL",
            "name": "细节决定成败",
            "postedtime": "2017/3/15",
            "commentcontent": "地球已经危在旦夕..."
        },
        {
            "head": "URL",
            "name": "细节决定成败",
            "postedtime": "2017/3/15",
            "commentcontent": "地球已经危在旦夕..."
        },
        {
            "head": "URL",
            "name": "细节决定成败",
            "postedtime": "2017/3/15",
            "commentcontent": "地球已经危在旦夕..."
        }
    ]
	},
	"resultCode": 1
}
```
 **返回参数说明** 

|参数名|类型|说明|
|:-----  |:-----|-----                           |
|videoimgURL |string   |视频图片url地址  |
|videoURl |string |视频播放url 路径 |
|title |string |返回详情标题 |
|content |string |返回详情内容 |
|price |number |返回打折后价格 |
|discount |number |返回打折前价格 |
|crowd |string |适合人群 |
|videolength |number |返回总视频数量 |
|timelength |number |返回总播放时长 |
|themecount |string |返回主题列表集数 |
|themetile |string |返回主题标题 |
|head |string |返回头像图片URL |
|name |string |返回用户名称 |
|postedtime |string |返回评论时间 |
|commentcontent |string  |返回评论内容 |

 **备注** 

- 更多返回错误代码请看首页的错误代码描述


