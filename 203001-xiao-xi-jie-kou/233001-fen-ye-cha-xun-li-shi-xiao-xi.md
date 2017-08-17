# 2.3、分页查询历史消息接口

* ### 接口名称

```
/api/im/getMsgListByPageAndUserId
```

### 接口方式

```
GET
```

* ### 接口参数

| 参数名 | 类型 | 说明 |
| :--- | :--- | :--- |
| appid | String | 接入应用CODE;目前项目使用 JH |
| page | String | 分页开始页；默认1 |
| limit | String | 每页显示记录条数；10条； |
| from | String | 发起查询的用户id |
| to | String | 对方的用户id |
| fromrole | String | 发起查询的用户角色；MEMBER:会员；SALER:客服销售 |
| lasttime | String | 13位时间戳；从哪个时间点开始查询对应的消息记录； |

* ### 返回参数

| 参数名 | 类型 | 说明 |
| :--- | :--- | :--- |
| success | String | true:成功；false:失败； |
| data数据格式如下： |  |  |
| from | String | 发送消息用户id |
| fromarea | String | 发送消息用户地区或者IP |
| fromrole | String | 发送消息用户角色；MEMBER:会员；SALER:客服销售 |
| f\_nickname | String | 发送消息用户昵称 |
| f\_avatar | String | 发送消息用户头像 |
| to | String | 接收消息用户ID |
| t\_nickname | String | 接收消息用户昵称 |
| t\_avatar | String | 接收消息用户头像 |
| torole | String | 接收消息用户角色；MEMBER:会员；SALER:客服销售 |
| content | String | 消息内容 |
| appid | String | 接入应用CODE;目前项目使用 JH |
| type | String | 消息类型；TEXT：文本消息；IMAGE：图片；VOICE消息：音频消息 |
| status | Number | 消息状态；0：未读；1：已读； |
| channel | String | 消息发送渠道；PC:电脑端；WX:微信端 |
| voiceLength | Number | 如果消息类型为：VOICE：存音频时长；否则默认-1 |
| imageSize | Number | 如果消息类型为：IMAGE，存图片大小；否则默认为-1 |
| sendtime | Number | 13位时间戳；消息发送时间； |
| readtime | Number | 13位时间戳；消息已读时间； |
| create\_at | String | 日期时间显示；消息创建时间； |

```
{
   "success": true,
   "data":    [
            {
         "_id": "5993a4fd3a9bc75c1cb2f64f",
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
         "sendtime": 1502877053329,
         "update_at": "2017-08-16T09:50:53.329Z",
         "create_at": "2017-08-16T09:50:53.329Z",
         "imageSize": -1,
         "voiceLength": -1,
         "channel": "PC",
         "torole": "SALER",
         "fromrole": "MEMBER",
         "type": "TEXT",
         "status": 0
      },
            {
         "_id": "5993a4fd3a9bc75c1cb2f64e",
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
         "sendtime": 1502877053003,
         "update_at": "2017-08-16T09:50:53.003Z",
         "create_at": "2017-08-16T09:50:53.003Z",
         "imageSize": -1,
         "voiceLength": -1,
         "channel": "PC",
         "torole": "SALER",
         "fromrole": "MEMBER",
         "type": "TEXT",
         "status": 0
      },
            {
         "_id": "5993a4fc3a9bc75c1cb2f64d",
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
         "sendtime": 1502877052635,
         "update_at": "2017-08-16T09:50:52.635Z",
         "create_at": "2017-08-16T09:50:52.635Z",
         "imageSize": -1,
         "voiceLength": -1,
         "channel": "PC",
         "torole": "SALER",
         "fromrole": "MEMBER",
         "type": "TEXT",
         "status": 0
      },
            {
         "_id": "5993a4fc3a9bc75c1cb2f64c",
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
         "sendtime": 1502877052067,
         "update_at": "2017-08-16T09:50:52.067Z",
         "create_at": "2017-08-16T09:50:52.067Z",
         "imageSize": -1,
         "voiceLength": -1,
         "channel": "PC",
         "torole": "SALER",
         "fromrole": "MEMBER",
         "type": "TEXT",
         "status": 0
      },
            {
         "_id": "5993a4fb3a9bc75c1cb2f64b",
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
         "sendtime": 1502877051061,
         "update_at": "2017-08-16T09:50:51.061Z",
         "create_at": "2017-08-16T09:50:51.061Z",
         "imageSize": -1,
         "voiceLength": -1,
         "channel": "PC",
         "torole": "SALER",
         "fromrole": "MEMBER",
         "type": "TEXT",
         "status": 0
      },
            {
         "_id": "5993a4f93a9bc75c1cb2f64a",
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
         "sendtime": 1502877049258,
         "update_at": "2017-08-16T09:50:49.258Z",
         "create_at": "2017-08-16T09:50:49.258Z",
         "imageSize": -1,
         "voiceLength": -1,
         "channel": "PC",
         "torole": "SALER",
         "fromrole": "MEMBER",
         "type": "TEXT",
         "status": 0
      },
            {
         "_id": "5993a3f8db6684a0137cca0d",
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
         "sendtime": 1502876643794,
         "update_at": "2017-08-16T09:44:03.794Z",
         "create_at": "2017-08-16T09:44:03.794Z",
         "imageSize": -1,
         "voiceLength": -1,
         "channel": "PC",
         "torole": "SALER",
         "fromrole": "MEMBER",
         "type": "TEXT",
         "status": 0
      },
            {
         "_id": "5993a3f9db6684a0137cca0e",
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
         "sendtime": 1502876643794,
         "update_at": "2017-08-16T09:44:03.794Z",
         "create_at": "2017-08-16T09:44:03.794Z",
         "imageSize": -1,
         "voiceLength": -1,
         "channel": "PC",
         "torole": "SALER",
         "fromrole": "MEMBER",
         "type": "TEXT",
         "status": 0
      },
            {
         "_id": "5993a402db6684a0137cca0f",
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
         "sendtime": 1502876643794,
         "update_at": "2017-08-16T09:44:03.794Z",
         "create_at": "2017-08-16T09:44:03.794Z",
         "imageSize": -1,
         "voiceLength": -1,
         "channel": "PC",
         "torole": "SALER",
         "fromrole": "MEMBER",
         "type": "TEXT",
         "status": 0
      },
            {
         "_id": "5993a405db6684a0137cca10",
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
         "sendtime": 1502876643794,
         "update_at": "2017-08-16T09:44:03.794Z",
         "create_at": "2017-08-16T09:44:03.794Z",
         "imageSize": -1,
         "voiceLength": -1,
         "channel": "PC",
         "torole": "SALER",
         "fromrole": "MEMBER",
         "type": "TEXT",
         "status": 0
      },
            {
         "_id": "5993a406db6684a0137cca11",
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
         "sendtime": 1502876643794,
         "update_at": "2017-08-16T09:44:03.794Z",
         "create_at": "2017-08-16T09:44:03.794Z",
         "imageSize": -1,
         "voiceLength": -1,
         "channel": "PC",
         "torole": "SALER",
         "fromrole": "MEMBER",
         "type": "TEXT",
         "status": 0
      },
            {
         "_id": "5993a407db6684a0137cca12",
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
         "sendtime": 1502876643794,
         "update_at": "2017-08-16T09:44:03.794Z",
         "create_at": "2017-08-16T09:44:03.794Z",
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



