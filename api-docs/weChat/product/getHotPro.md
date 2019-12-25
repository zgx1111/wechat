## 查看热点商品 /wechat/product/getHotPro/

- **`HTTPS 请求方式`** GET

## Example Request
```
https://{host}/api/v1/product/WxGetHotPro
```

## Request Parameter

| 参数名       | 必选   | 参数对应值 | 说明                  |
| ------------ | ------ | ---------- | --------------------|
| store        | `true` | `int    `  | 门店id              |


## Request Body
```
{
    "store":1
}
```

## Response Parameter

| 参数名              | 必选   | 参数对应值 | 说明                              |
| ------------------- | ------ | ---------- | --------------------------------|
| id                  | `true` | `int    `  | 主键id                          |
| name                | `true` | `string`   | 商品名字                         |
| price               | `true` | `int`      | 价格                             |
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
[    
{
        "id": 266,
        "name": "霏慕诱惑开裆免脱连裤袜透视半身袜7305黑色",
        "price": "16.60",
        "cost": "0.00",
        "stock": 999,
        "state": 1,
        "sales":0,
        "delete_time": null,
        "category_id": 5,
        "main_img_url": "http://z.cn/images/20191215/2bb2226ddb4e10bdd3806d311370becf.jpg",
        "create_time": "2019-12-15 17:33:24",
        "update_time": "2019-12-15 17:33:24",
        "img_id": 1345,
        "storehouse_id": 6,
        "imgs": [
            {
                "id": 976,
                "img_id": 1346,
                "product_id": 266,
                "img_url": {
                    "url": "http://z.cn/images/20191215/66d91f636bb55bc121093ea88633bb5e.jpg",
                    "create_time": "2019-12-15 17:34:15"
                }
            },
            {
                "id": 977,
                "img_id": 1347,
                "product_id": 266,
                "img_url": {
                    "url": "http://z.cn/images/20191215/e1a48704a7ec85d70f53827eb5715fc6.jpg",
                    "create_time": "2019-12-15 17:34:20"
                }
            }
        ],
         "main_imgs": [
            {
                "id": 241,
                "img_id": 1731,
                "product_id": 264,
                "img_url": {
                    "url": "http://yxadult.xyz/images/20191221/82fc7db48fdcda421eedd4044d97e211.jpg",
                    "create_time": "2019-12-21 11:34:04"
                }
            },
            {
                "id": 241,
                "img_id": 1731,
                "product_id": 264,
                "img_url": {
                    "url": "http://yxadult.xyz/images/20191221/82fc7db48fdcda421eedd4044d97e211.jpg",
                    "create_time": "2019-12-21 11:34:04"
                }
            }

        ]
    },
    {
        "id": 265,
        "name": "柠檬物语套装秘书学生制服性感白衣黑裙职业套装8154",
        "price": "89.00",
        "cost": "0.00",
        "stock": 999,
        "sales":0,
        "state": 1,
        "delete_time": null,
        "category_id": 5,
        "main_img_url": "http://z.cn/images/20191215/e0c449cd8583cba2598c184f6f439c68.jpg",
        "create_time": "2019-12-15 17:19:32",
        "update_time": "2019-12-15 17:19:32",
        "img_id": 1341,
        "storehouse_id": 6,
        "imgs": [
            {
                "id": 973,
                "img_id": 1342,
                "product_id": 265,
                "img_url": {
                    "url": "http://z.cn/images/20191215/b780b3ed41e158478164734b13a93bdf.jpg",
                    "create_time": "2019-12-15 17:19:52"
                }
            },
            {
                "id": 974,
                "img_id": 1343,
                "product_id": 265,
                "img_url": {
                    "url": "http://z.cn/images/20191215/c560e64ade22f66133be416812d3bff4.jpg",
                    "create_time": "2019-12-15 17:19:58"
                }
            }
        ],
        "main_imgs": []
    }
]
```

