## 获得已付款订单 /cms/order/getOederRemind
- **`HTTPS 请求方式`** POST

## Example Request
```
https://{host}/api/v1/order/getOrderRemind
```

## Request Parameter

| 参数名        | 必选   | 参数对应值  | 说明                            |    
| ------------ | ------ | ---------- | --------------------------------|
| page         | `true` | `int`      | 页数，默认第一页                 |


## Request Body

```
token在header里传

{
    "page":1,
}

```



## Response Parameter

| 参数名              | 必选   | 参数对应值 | 说明                                     |
| ------------------- | ------ | ---------- | ---------------------------------      |
| id                  | `true` | `int`      | 订单id                            		 |
| order_no            | `true` | `string`   | 订单号                            		 |
| create_time         | `true` | `string`   | 创建时间                          		 |
| total_price         | `true` | `int`      | 总价格                            		 |
| status              | `true` | `int`      | 订单状态：1是未付款，2是已支付，3是已发货  |
| remarks             | `true` | `string`   | 订单备注                                |
| send_time           | `true` | `string`   | 订单发货时间                            |
| snap_img            | `true` | `string`   | 订单图片                           	 |
| snap_name           | `true` | `string`   | 订单名字                           	 |
| total_count         | `true` | `int`      | 订单总数量                         	 |
| storehouse_id       | `true` | `int`      | 订单所属供货仓id                   	 	 |
| store_id            | `true` | `int`      | 订单所属门店id                     		 |
| snap_items          | `true` | `int`      | 订单内容                                |
| snap_address        | `true` | `int`      | 订单地址                                |


## Response Body

```
有订单：
[
    {
        "id": 10,
        "order_no": "AC31794351911755",
        "send_time": "2019-12-31",
        "create_time": "2019-12-31 16:03:55",
        "total_price": "0.02",
        "status": 1,
        "remarks": "斯达克警方和",
        "snap_img": "https://yxadult.xyz/images/20191227/ec0acbf941bcafb38db28d673ce61315.jpg",
        "snap_name": "1等",
        "total_count": 1,
        "snap_items": [
            {
                "id": 596,
                "haveStock": true,
                "counts": "1",
                "price": "0.02",
                "name": "1",
                "totalPrice": 0.02,
                "main_img_url": "https://yxadult.xyz/images/20191227/ec0acbf941bcafb38db28d673ce61315.jpg"
            }
        ],
        "snap_address": {
            "name": "赵",
            "phone": "18747830783",
            "store_id": "1",
            "address": "你那",
            "create_time": "2019-12-17 12:56:41",
            "update_time": "2019-12-21 15:25:02"
        },
        "prepay_id": null,
        "storehouse_id": 8,
        "store_id": 54,
        "store": {
            "id": 54,
            "username": "cs100",
            "password": "123",
            "truename": "测试",
            "state": 1,
            "storehouse_id": 8,
            "city_id": "1",
            "address": "sd",
            "amount": 0,
            "eworker_id": 1,
            "phone": "13923879876",
            "create_time": "2019-12-27 10:12:58",
            "update_time": "2019-12-27 10:24:04",
            "delete_time": null
        }
    },
]

无订单：
[]

```

