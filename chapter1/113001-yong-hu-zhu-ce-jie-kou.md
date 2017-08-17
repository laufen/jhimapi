# 1.1、用户注册接口

* ### 接口名称

```
/api/im/regUserInfo
```

* ### 接口参数

| 参数名 | 类型 | 说明 |
| :--- | :--- | :--- |
| appid | String | 接入应用CODE;目前项目使用 JH |
| userid | String | 注册的用户id |
| userrole | String | 用户角色；MEMBER:会员；SALER:客服销售 |
| channel | String | 注册渠道；PC:电脑端；WX:微信端 |

* ### 返回参数

| 参数名 | 类型 | 说明 |
| :--- | :--- | :--- |
| success | String | true:成功；false:失败； |

```
{
   "success": true,
   "data":    {
      "n": 1,
      "nModified": 1,
      "ok": 1
   }
}
```



