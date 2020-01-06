## 供货仓登陆 /cms/login/storehouseLogin
- **`HTTPS 请求方式`** POST

## Example Request
```
https://{host}/api/v1/storehouse
```

## Request Parameter

| 参数名        | 必选   | 参数对应值  | 说明                            |    
| ------------ | ------ | ---------- | --------------------------------|
| username     | `true` | `int`      | 账号                            |
| password     | `true` | `int`      | 密码                            |


## Request Body

```
token在header里传

{
    "username":1123,
    "password":213
}

```



## Response Parameter

| 参数名              | 必选   | 参数对应值 | 说明                                     |
| ------------------- | ------ | ---------- | ---------------------------------      |
| status              | `true` | `int`      | 返回状态                         		 |
| token               | `true` | `int`      | 令牌                                    |



## Response Body

```
成功：
{
    "status": 1,
    "token": "cddfeb420add9e9b4b90e2abacc6a3b2"
}


失败：
{
    "msg": "授权失败",
    "errorCode": 10004,
    "request_url": "/api/v1/storehouse?username=wuchang101&password=1234"
}

```

