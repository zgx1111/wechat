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
| time         | `true` | `string`   | 送货时间              |
| remarks      | `true` | `string`   | 备注                 |

## Request Body

```
token在header里传

{
	
	"products":[
			{"product_id": 222, "count": 1}
		],
	"store":1,
	"time":8:00,
    "remarks":"数据库的杀菌的"

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
	"total_price": 157.6,
	pass: true,

}


失败：

{
    "pass": false,
    "orderPrice": 292.6,
    "totalCount": 11,
    "pStatusArray": [
        {
            "id": 55,
            "haveStock": false,
            "counts": "11",
            "price": "26.60",
            "name": "名流避孕套爽口套 樱桃味 10只装",
            "totalPrice": 292.6,
            "main_img_url": "http://z.cn/images/20191221/d047e22e1e26a76b7daf4976b84d8d35.jpg"
        }
    ],
    "order_id": -1
}

```

