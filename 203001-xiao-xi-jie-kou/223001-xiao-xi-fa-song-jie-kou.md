# 2.2、消息发送接口

* ### 接口名称

```
/api/im/sendMsg
```

* ### 接口方式

```
POST
```

* ### 接口参数（先调试文本消息）

| 参数名 | 类型 | 说明 |
| :--- | :--- | :--- |
| appid | String | 接入应用CODE;目前项目使用 JH |
| from | String | 发送消息用户id |
| fromarea | String | 发送消息用户地区或者IP |
| fromrole | String | 发送消息用户角色；MEMBER:会员；SALER:客服销售 |
| f\_nickname | String | 发送消息用户昵称 |
| f\_avatar | String | 发送消息用户头像 |
| to | String | 接收消息用户ID |
| t\_nickname | String | 接收消息用户昵称 |
| t\_avatar | String | 接收消息用户头像 |
| content | String | 消息内容 |
| type | String | 消息类型；TEXT：文本消息；IMAGE：图片；VOICE消息：音频消息 |
| channel | String | 消息发送渠道；PC:电脑端；WX:微信端 |
| bustype | String | 业务对象类型；CHAT: 普通聊天；GOOD\_CHAT: 基于产品询价聊天； ORDER\_CHAT:基于订单聊天； |
| busid | String | 如果是非普通聊天类型；存放对应业务对象ID;例如：产品ID，订单ID |

* ### 返回参数

| 参数名 | 类型 | 说明 |
| :--- | :--- | :--- |
| success | String | true:成功；false:失败； |
| data数据格式如下：消息保存成功记录信息 |  |  |
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
   "data":    {
      "__v": 0,
      "busid": "34",
      "fromarea": "192.",
      "content": "ffffffffff",
      "t_avatar": "to.jpg",
      "t_nickname": "ikima",
      "to": "2",
      "f_avatar": "FTOM.jpg",
      "f_nickname": "LAUFEN",
      "from": "200",
      "appid": "JH",
      "_id": "599555d9ff149c68091c8b8e",
      "readtime": -1,
      "sendtime": 1502987865961,
      "update_at": "2017-08-17T16:37:45.961Z",
      "create_at": "2017-08-17T16:37:45.961Z",
      "imageSize": -1,
      "voiceLength": -1,
      "channel": "PC",
      "torole": "SALER",
      "fromrole": "MEMBER",
      "bustype": "GOOD_CHAT",
      "type": "TEXT",
      "status": 0
   }
}
```



