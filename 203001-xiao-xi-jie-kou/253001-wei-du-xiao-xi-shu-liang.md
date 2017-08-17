### 2.5、未读消息数量

* ### 接口名称

```
/api/im/unreadcount
```

* ### 接口方式

```
GET
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
| success | boolean | true:成功；false:失败； |
| data | int | 未读消息数量 |

```
{
   "success": true,
   "data": 5
}
```



