## 订单支付 /wechat/order/pre_order
- **`HTTPS 请求方式`** POST

## Example Request
```
https://{host}/api/v1/pay/pre_order  
```

## Request Parameter

| 参数名       | 必选   | 参数对应值 | 说明                  |
| ------------ | ------ | ---------- | --------------------|
| id           | `true` | `int`      | 订单id               |
| store        | `true` | `int`      | 门店id               |


## Request Body

```
token在header里传

{
	
	"id":订单id,
	"store":门店id

}
```



## Response Parameter

| 参数名              | 必选   | 参数对应值 | 说明                               |
| ------------------- | ------ | ---------- | ---------------------------------|
| appid               | `true` | `string`   | appid                            |
| nonceStr            | `true` | `string`   | 生成签名的随机串                   |
| package             | `true` | `string`   |                                   |
| signType            | `true` | `string`   | 加密方式md5                       |
| timeStamp           | `true` | `string`   | 生成签名的时间戳                   |


## Response Body

```
{
	appId: "wxd0eb1627548a8ca8", 
	nonceStr: "0aec17abaf5ae4ea20e187c49aad52c0", 
	package: "prepay_id=wx23115054544007bdeb278ca11576052800", 
	signType: "md5", 
	timeStamp: "1577072998"
}
```

