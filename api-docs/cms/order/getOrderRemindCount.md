## 获得付款订单数量 /cms/order/getOrderRemindCount
- **`HTTPS 请求方式`** POST

## Example Request
```
https://{host}/api/v1/order/getOrderRemindCount

```

## Request Parameter

| 参数名       | 必选   | 参数对应值 | 说明                  |
| ------------ | ------ | ---------- | --------------------|


## Request Body

```
token在header里传

```



## Response Parameter

| 参数名              | 必选   | 参数对应值 | 说明                                     |
| ------------------- | ------ | ---------- | ---------------------------------      |
| count               | `true` | `int`      | 订单数量                         		 |
| status              | `true` | `boolea`   | 返回状态                         		 |



## Response Body

```
{
    "count": 10,
    "status": true
}




```

