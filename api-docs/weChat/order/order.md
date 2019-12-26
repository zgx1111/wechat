## 下订单 /wechat/order/order
- **`HTTPS 请求方式`** POST

## Example Request
```
https://{host}/api/v1/order
```

## Request Parameter

| 参数名       | 必选   | 参数对应值 | 说明                  |
| ------------ | ------ | ---------- | --------------------|
| products     | `true` | `array`    | 商品数组             |
| product_id   | `true` | `int`      | 商品id               |
| count        | `true` | `int`      | 商品数量             |
| store        | `true` | `int`      | 门店id               |
| time         | `true` | `int`      | 送货时间              |

## Request Body

```
token在header里传

{
	
	"products":[
			{"product_id": 222, "count": 1}
		],
	"store":1,
	"time":8

}
```



## Response Parameter

| 参数名              | 必选   | 参数对应值 | 说明                               |
| ------------------- | ------ | ---------- | ---------------------------------|
| order_no            | `true` | `string`   | 订单号                            |
| order_id            | `true` | `int`      | 订单id                            |
| create_time         | `true` | `string`   | 创建时间                          |
| pass                | `true` | `Boolen`   | 订单是否创建                      |


## Response Body

```
成功：

{
	order_no: "AC23680855028905", 
	order_id: "82", 
	create_time: "2019-12-23 10:28:05", 
	pass: true

}


失败：

{
	"order_id":-1,
	"pass":false
}

```

