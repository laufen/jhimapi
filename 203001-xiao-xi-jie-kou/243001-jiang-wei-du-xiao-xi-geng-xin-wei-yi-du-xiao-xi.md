### 2.4、消息状态更接口

> ### 将未读消息更新为已读

* ### 接口名称

```
接口名称/api/im/updateUnreadP2pMessages
```

* ### 接口方式

```
POST
```

* ### 接口参数

| 参数名 | 类型 | 说明 |
| :--- | :--- | :--- |
| appid | String | 接入应用CODE;目前项目使用 JH |
| from | String | 发送消息用户id |
| fromrole | String | 发送消息用户角色；MEMBER:会员；SALER:客服销售 |
| to | String | 接收消息用户ID |

* ### 返回参数

| 参数名 | 类型 | 说明 |
| :--- | :--- | :--- |
| success | String | true:成功；false:失败； |
| data数据格式如下：消息保存成功记录信息 |  |  |
| nModified | String | 更新记录条数 |
| ok | String | 更新成功或者失败；1：成功； |

```
{
   "success": true,
   "data":    {
      "n": 17,
      "nModified": 17,
      "ok": 1
   }
}
```



