## 用户获得地址 /wechat/address/getAddress/

- **`HTTPS 请求方式`** GET

## Example Request
```
https://yxadult.xyz/api/v1/address
```

## Request Parameter

| 参数名       | 必选   | 参数对应值 | 说明                  |
| ------------ | ------ | ---------- | --------------------|
| token        | `true` | `string`   | token令牌            |


## Request Body

```
从header中传token


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


    {
        "name": "hao",
        "phone": "18723456789",
        "store_id": "1",
        "address": "dsa",
        "create_time": "2019-12-17 13:08:06",
        "update_time": "2019-12-17 13:08:06"
   }




```

