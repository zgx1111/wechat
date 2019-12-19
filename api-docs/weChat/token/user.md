## 微信获得token令牌 /wechat/token/user/

- **`HTTPS 请求方式`** POST

## Example Request
```
https://yxadult.xyz/api/v1/token/user
```

## Request Parameter

| 参数名       | 必选   | 参数对应值 | 说明                  |
| ------------ | ------ | ---------- | --------------------|
| code         | `true` | `string`   | 微信code            |


## Request Body
```
{
	"code":011huWZo0kxYho1YIh0p0kj40p0huWZo
}

```
## Response Parameter

| 参数名              | 必选   | 参数对应值 | 说明                              |
| ------------------- | ------ | ---------- | --------------------------------|
| token               | `true` | `string`   | token令牌                       |


## Response Body

```
{
    "token": "1f227cab89598a5f92ad03b8379fd1d0"
}
```

