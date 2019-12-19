## 用户添加或者更新地址 /wechat/address/setAddress/

- **`HTTPS 请求方式`** POST

## Example Request
```
https://yxadult.xyz/api/v1/address
```

## Request Parameter

| 参数名       | 必选   | 参数对应值 | 说明                  |
| ------------ | ------ | ---------- | --------------------|
| token        | `true` | `string`   | token令牌            |
| name         | `true` | `string`   | 姓名                 |
| phone        | `true` | `int`      | 电话                 |
| store        | `true` | `int`      | 门店id               |
| address      | `true` | `string`   | 详细地址              |


## Request Body


```
从header中传token


{
	"name":'213',
	"phone":123213123,
	"store":1,
	"address":"的撒飒飒倒萨的撒旦"
}


```


## Response Parameter



| 参数名              | 必选   | 参数对应值 | 说明                              |
| -------------------| ------ | ---------- | --------------------------------|
| name               | `true` | `string`   | 用户名字                         |
| phone              | `true` | `int`      | 用户电话                         |
| store_id           | `true` | `int`      | 门店id                           |
| address            | `true` | `string`   | 详细地址                         |
| create_time        | `true` | `string`   | 创建时间                         |
| update_time        | `true` | `string`   | 更新时间                         |



## Response Body

```
成功

{
    "status": true,
    "addressID": 10
}

失败

{
    "status": false,
    "addressID": 0
}


```

