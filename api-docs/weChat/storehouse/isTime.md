## 查看是否在营业时间 /wechat/storehouse/isTime/

- **`HTTPS 请求方式`** GET

## Example Request
```
https://yxadult.xyz/api/v1/storehouse/isTime
```

## Request Parameter

| 参数名       | 必选   | 参数对应值 | 说明                  |
| ------------ | ------ | ---------- | --------------------|
| store        | `true` | `int   `   | 门店id           |


## Request Body

```
{
    "store":1
}
```



## Response Parameter

| 参数名              | 必选   | 参数对应值 | 说明                               |
| ------------------- | ------ | ---------- | ---------------------------------|
| status              | `true` | `Boolean`  | 返回状态                          |


## Response Body

```
在营业时间内:

{
    "status": true
}


不在营业时间内：
{
    'status'=>false,
    'begin'=>8,
    'end'=>12
}

```

