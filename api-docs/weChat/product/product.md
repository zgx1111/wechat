## 查看某个商品详细信息 /wechat/product/product/

- **`HTTPS 请求方式`** GET

## Example Request
```
https://{host}/api/v1/product/:id
```

## Request Parameter

| 参数名       | 必选   | 参数对应值 | 说明                  |
| ------------ | ------ | ---------- | --------------------|



## Request Body

## Response Parameter

| 参数名              | 必选   | 参数对应值 | 说明                              |
| ------------------- | ------ | ---------- | --------------------------------|
| id                  | `true` | `int    `  | 主键id                          |
| name                | `true` | `string`   | 商品名字                         |
| price               | `true` | `int`      | 价格                             |
| sprice               | `true` | `int`     | 特殊价格                         |
| limit_count         | `true` | `int`      | 限制数量，特价的限制数量，买了就会减少，小于等于0时恢复原价 |
| discount            | `true` | `int`      | 折扣                             |
| cost                | `true` | `int`      | 成本                             |
| stock               | `true` | `int`      | 存货                             |
| sales               | `true` | `int`      | 销量                             |
| state               | `true` | `int`      | 状态，1是上架，0是下架            |
| create_time         | `true` | `int`      | 创建时间                         |
| update_time         | `true` | `int`      | 更新时间                         |
| delete_time         | `true` | `int`      | 删除时间                         |
| category_id         | `true` | `int`      | 分类id                           |
| summary             | `true` | `string`   | 商品简述                         |
| storehouse_id       | `true` | `int`      | 供货仓id                         |
| imgs                | `true` | `array`    | 副图片数组                        |
| main_imgs           | `true` | `array`    | 主图片数组                        |
| main_img_url        | `true` | `string`   | 主图片url:即将弃用                |
| img_id              | `true` | `int`      | 主图片id:即将弃用                 |
## Response Body

```
{
    "id": 237,
    "name": "谜姬二代加温久潮男用后霆振动棒12频USB充电",
    "price": "218.00",
    "sprice": null,
    "limit_counts": 196,
    "discount": "1.00",
    "cost": "0.00",
    "stock": 100,
    "sales": 0,
    "state": 1,
    "delete_time": null,
    "category_id": 9,
    "main_img_url": "http://z.cn/images/20191221/967dc2dfdd56bdc6ff4793343d60a72d.jpg",
    "create_time": "2019-12-14 17:30:26",
    "update_time": "2019-12-21 11:18:29",
    "summary": "",
    "img_id": 992,
    "storehouse_id": 6,
    "imgs": [
        {
            "id": 652,
            "img_id": 993,
            "product_id": 237,
            "img_url": {
                "url": "http://z.cn/images/20191214/47dfd393912e2cf54270ffeb6adac2b1.jpg",
                "create_time": "2019-12-14 17:30:45"
            }
        },
        {
            "id": 653,
            "img_id": 994,
            "product_id": 237,
            "img_url": {
                "url": "http://z.cn/images/20191214/0dbcbd25a04290a5a57a0af3cf5646f2.jpg",
                "create_time": "2019-12-14 17:30:49"
            }
        },
        {
            "id": 654,
            "img_id": 995,
            "product_id": 237,
            "img_url": {
                "url": "http://z.cn/images/20191214/6f9cfd9f2465d2123e1eca4ddf9bcd9b.jpg",
                "create_time": "2019-12-14 17:31:00"
            }
        },
        {
            "id": 655,
            "img_id": 996,
            "product_id": 237,
            "img_url": {
                "url": "http://z.cn/images/20191214/5b4b13f81ef480dc0bb52b9ab3e65e0f.jpg",
                "create_time": "2019-12-14 17:31:18"
            }
        },
        {
            "id": 656,
            "img_id": 997,
            "product_id": 237,
            "img_url": {
                "url": "http://z.cn/images/20191214/d024171f3da8e82fefcd7333e2396b05.jpg",
                "create_time": "2019-12-14 17:31:21"
            }
        }
    ],
    "main_imgs": [
        {
            "id": 231,
            "img_id": 1700,
            "product_id": 237,
            "img_url": {
                "url": "http://z.cn/images/20191221/967dc2dfdd56bdc6ff4793343d60a72d.jpg",
                "create_time": "2019-12-21 11:18:27"
            }
        }
    ]
}
```

