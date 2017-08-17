* # 2.2、获取用户状态
* ### 接口名称

```
/api/im/getUserStatus
```

* ### 接口参数

| 参数名 | 类型 | 说明 |
| :--- | :--- | :--- |
| appid | String | 接入应用CODE;目前项目使用 JH |
| userid | String | 注册的用户id |
| userrole | String | 用户角色；MEMBER:会员；SALER:客服销售 |

* ### 返回参数

| 参数名 | 类型 | 说明 |
| :--- | :--- | :--- |
| success | String | true:成功；false:失败； |
| isonline | Int | 是否在线；1：在线； 0：离线 |
| heartime | Number | 心跳时间戳；13位； |
| update\_at | String | 最新心跳时间展示； |

```
{
   "success": true,
   "data": [   {
      "_id": "5994140b77ac357c02ae96a5",
      "userarea": "",
      "userid": "200",
      "appid": "JH",
      "__v": 0,
      "update_at": "2017-08-17T09:40:59.306Z",
      "create_at": "2017-08-16T17:44:43.750Z",
      "isonline": 1,
      "hearttime": 1502962859306,
      "channel": "",
      "userrole": "MEMBER"
   }]
}
```



