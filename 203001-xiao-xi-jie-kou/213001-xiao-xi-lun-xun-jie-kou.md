# 2.1、消息轮询接口

* ### 接口名称

```
/api/im/getNewestMsgListByLastTime
```

### 接口方式

```
GET
```

* ### 接口参数

| 参数名 | 类型 | 说明 |
| :--- | :--- | :--- |
| appid | String | 接入应用CODE;目前项目使用 JH |
| from | String | 发起查询的用户id |
| to | String |  |
| fromrole |  |  |
| lasttime | String |  |

* ### 返回参数

| 参数名 | 类型 | 说明 |
| :--- | :--- | :--- |
| success | String | true:成功；false:失败； |

```
{
   "success": true,
   "data":    [
            {
         "_id": "5993a4ff3a9bc75c1cb2f653",
         "fromarea": "192.",
         "content": "ffffffffff",
         "t_avatar": "to.jpg",
         "t_nickname": "ikima",
         "to": "2",
         "f_avatar": "FTOM.jpg",
         "f_nickname": "LAUFEN",
         "from": "200",
         "appid": "JH",
         "__v": 0,
         "readtime": -1,
         "sendtime": 1502877055334,
         "update_at": "2017-08-16T09:50:55.334Z",
         "create_at": "2017-08-16T09:50:55.334Z",
         "imageSize": -1,
         "voiceLength": -1,
         "channel": "PC",
         "torole": "SALER",
         "fromrole": "MEMBER",
         "type": "TEXT",
         "status": 0
      },
            {
         "_id": "5993a4fe3a9bc75c1cb2f652",
         "fromarea": "192.",
         "content": "ffffffffff",
         "t_avatar": "to.jpg",
         "t_nickname": "ikima",
         "to": "2",
         "f_avatar": "FTOM.jpg",
         "f_nickname": "LAUFEN",
         "from": "200",
         "appid": "JH",
         "__v": 0,
         "readtime": -1,
         "sendtime": 1502877054675,
         "update_at": "2017-08-16T09:50:54.675Z",
         "create_at": "2017-08-16T09:50:54.675Z",
         "imageSize": -1,
         "voiceLength": -1,
         "channel": "PC",
         "torole": "SALER",
         "fromrole": "MEMBER",
         "type": "TEXT",
         "status": 0
      }
   ]
}
```



