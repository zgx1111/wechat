## 获得用户全部订单 /wechat/order/getOederByUser
- **`HTTPS 请求方式`** GET

## Example Request
```
https://{host}/api/v1/order/by_user
```

## Request Parameter

| 参数名        | 必选   | 参数对应值  | 说明                            |    
| ------------ | ------ | ---------- | --------------------------------|
| page         | `true` | `int`      | 页数，默认第一页                 |
| size         | `true` | `int`      | 每页的订单数量，默认一页15个      |


## Request Body

```
token在header里传

参数可传可不传
{
    "page":1,
    "size":15
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
| snap_img            | `true` | `string`   | 订单图片                           	 |
| snap_name           | `true` | `string`   | 订单名字                           	 |
| total_count         | `true` | `int`      | 订单总数量                         	 |
| storehouse_id       | `true` | `int`      | 订单所属供货仓id                   	 	 |
| store               | `true` | `int`      | 订单所属门店id                     		 |
| current_page        | `true` | `int`      | 当前页码                                |


## Response Body

```
{
    "data": [
        {
            "id": 95,
            "order_no": "AC23853294722181",
            "create_time": "2019-12-23 15:15:29",
            "total_price": "79.80",
            "status": 1,
            "snap_img": "http://yxadult.xyz/images/20191220/51640bdb2966bc7453cf16690b62422f.jpg",
            "snap_name": "霏慕性感蕾丝花边丝袜吊袜带一体连裤袜7361肉色等",
            "total_count": 2,
            "storehouse_id": 6,
            "store_id": 1
        },
        {
            "id": 94,
            "order_no": "AC23851813384563",
            "create_time": "2019-12-23 15:13:01",
            "total_price": "79.80",
            "status": 1,
            "snap_img": "http://yxadult.xyz/images",
            "snap_name": "霏慕性感蕾丝花边丝袜吊袜带一体连裤袜7361肉色等",
            "total_count": 2,
            "storehouse_id": 6,
            "store_id": 1
        }
     
    ],
    "current_page": 1
}

```

