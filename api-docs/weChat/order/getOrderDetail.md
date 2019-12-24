## 获得订单详情 /wechat/order/getOederDetail
- **`HTTPS 请求方式`** GET

## Example Request
```
https://{host}/api/v1/order/:id
```

## Request Parameter

| 参数名       | 必选   | 参数对应值 | 说明                  |
| ------------ | ------ | ---------- | --------------------|
| id           | `true` | `int`      | 订单id              |


## Request Body

```
token在header里传

```



## Response Parameter

| 参数名              | 必选   | 参数对应值 | 说明                                     |
| ------------------- | ------ | ---------- | ---------------------------------      |
| id                  | `true` | `int`      | 订单id                            		 |
| order_no            | `true` | `string`   | 订单号                            		 |
| create_time         | `true` | `string`   | 创建时间                          		 |
| total_price         | `true` | `int`      | 总价格                            		 |
| status              | `true` | `int`      | 订单状态：1是未付款，2是已支付，3是已发货  |
| snap_img            | `true` | `string`   | 订单图片                           	 |
| snap_name           | `true` | `string`   | 订单名字                           	 |
| total_count         | `true` | `int`      | 订单总数量                         	 |
| snap_items          | `true` | `array`    | 订单商品                           	 |
| snap_address        | `true` | `string`   | 订单地址                           	 |
| storehouse_id       | `true` | `int`      | 订单所属供货仓id                   	 	 |
| store               | `true` | `int`      | 订单所属门店id                     		 |
| haveStock           | `true` | `Boolen`   | 订单中商品是否有库存：true是有           |


## Response Body

```
{
    "id": 95,
    "order_no": "AC23853294722181",
    "create_time": "2019-12-23 15:15:29",
    "total_price": "79.80",
    "status": 1,
    "snap_img": "http://yxadult.xyz/images/20191220/51640bdb2966bc7453cf16690b62422f.jpg",
    "snap_name": "霏慕性感蕾丝花边丝袜吊袜带一体连裤袜7361肉色等",
    "main_img_url":"http://yxadult.xyz/images/20191220/51640bdb2966bc7453cf16690b62422f.jpg",
    "total_count": 2,
    "snap_items": [
        {
            "id": 270,
            "haveStock": true,
            "counts": "2",
            "price": "39.90",
            "name": "霏慕性感蕾丝花边丝袜吊袜带一体连裤袜7361肉色",
            "totalPrice": 79.8,
            "main_img_url": "http://yxadult.xyz/images/20191220/51640bdb2966bc7453cf16690b62422f.jpg"
        }
    ],
    "snap_address": {
        "name": "赵sad",
        "phone": "15044563215",
        "store_id": "1",
        "address": "县里dsada",
        "create_time": "2019-12-17 12:56:41",
        "update_time": "2019-12-19 17:22:55"
    },
    "storehouse_id": 6,
    "store_id": 1
}


```

