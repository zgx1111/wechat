## 接单 /cms/order/orderTaking 
- **`HTTPS 请求方式`** POST

## Example Request
```
https://{host}/api/v1/order/orderTaking
```

## Request Parameter

| 参数名        | 必选   | 参数对应值  | 说明                            |    
| ------------ | ------ | ---------- | --------------------------------|
| id           | `true` | `int`      | 订单id                          |


## Request Body

```
token在header里传
{
    "id":1,
}

```



## Response Parameter

| 参数名              | 必选   | 参数对应值 | 说明                                     |
| ------------------- | ------ | ---------- | ---------------------------------      |


## Response Body

```
成功：
    true

失败：
    false
```

