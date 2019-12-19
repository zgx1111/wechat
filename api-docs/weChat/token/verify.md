## 微信检验token令牌是否过期 /wechat/token/verify/

- **`HTTPS 请求方式`** POST

## Example Request
```
https://{host}/api/v1/token/verify
```

## Request Parameter

| 参数名       | 必选   | 参数对应值 | 说明                  |
| ------------ | ------ | ---------- | --------------------|
| token        | `true` | `string`   | token令牌           |


## Request Body
```
{
	"token":62c52a582096a24858c37173799a2224	
}
```
## Response Parameter

| 参数名              | 必选   | 参数对应值 | 说明                              |
| ------------------- | ------ | ---------- | --------------------------------|
| isValid             | `true` | `Boolean`  | token是否过期                    |


## Response Body

```

未过期：

{
    "isValid": true
}


过期：

{
    "isValid": false
}
```

