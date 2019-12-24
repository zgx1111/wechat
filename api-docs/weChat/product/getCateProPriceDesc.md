## 获得分类商品，价格倒序 /wechat/product/getCateProPriceDesc/

- **`HTTPS 请求方式`** GET

## Example Request
```
https://{host}/api/v1/product/getCateProPriceDesc
```

## Request Parameter

| 参数名       | 必选   | 参数对应值 | 说明                  |
| ------------ | ------ | ---------- | --------------------|
| store        | `true` | `int    `  | 门店id              |
| id           | `true` | `int    `  | 分类id              |

## Request Body

```
{
    "store":1，
    "id":1
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
        "id": 92,
        "name": "【情趣用品】人初油 金装加强版人初油男用喷剂 (金装人初油)\t",
        "price": "98.00",
        "cost": "18.00",
        "stock": 5,
        "sales": 0,
        "state": 1,
        "delete_time": null,
        "category_id": 1,
        "main_img_url": "http://cf.yxadult.xyz/images",
        "create_time": "2019-12-24 00:15:33",
        "update_time": "2019-12-24 00:15:33",
        "summary": "品牌：人初油\n品牌类型：国货品牌\n产品类别：情趣 - 男用喷剂-MP\n产品名称：人初油抑菌喷剂\n生产",
        "img_id": null,
        "storehouse_id": 1,
        "imgs": [
            {
                "id": 541,
                "img_id": 831,
                "product_id": 92,
                "img_url": {
                    "url": "http://cf.yxadult.xyz/images/20191224/be0f8b6e74070f39a6de3e3d571f34b0.jpg",
                    "create_time": "2019-12-24 00:12:09"
                }
            },
            {
                "id": 542,
                "img_id": 832,
                "product_id": 92,
                "img_url": {
                    "url": "http://cf.yxadult.xyz/images/20191224/f8e86194dedd29c8de074c5975efb1f7.jpg",
                    "create_time": "2019-12-24 00:12:28"
                }
            },
            
        ],
        "main_imgs": [
            {
                "id": 361,
                "img_id": 827,
                "product_id": 92,
                "img_url": {
                    "url": "http://cf.yxadult.xyz/images/20191224/aeab73b5f41a876af9a0f77d4c3606ae.png",
                    "create_time": "2019-12-24 00:11:21"
                }
            },
            {
                "id": 362,
                "img_id": 828,
                "product_id": 92,
                "img_url": {
                    "url": "http://cf.yxadult.xyz/images/20191224/e8299b871fb1b0430e27f448979a9bdc.jpg",
                    "create_time": "2019-12-24 00:11:31"
                }
            },
        ]
    },
    {
        "id": 14,
        "name": "【避孕套】杜蕾斯 情迷装 现改名为：爽薄情迷装",
        "price": "90.00",
        "cost": "30.00",
        "stock": 2,
        "sales": 0,
        "state": 1,
        "delete_time": null,
        "category_id": 1,
        "main_img_url": "http://cf.yxadult.xyz/images",
        "create_time": "2019-12-22 16:13:47",
        "update_time": "2019-12-22 16:13:47",
        "summary": "产品名称: 避孕套\r\n产品标准: GB7544\r\n产地: 大陆\r\n保质期: 5年\r\n品牌: Dure",
        "img_id": null,
        "storehouse_id": 1,
        "imgs": [
            {
                "id": 65,
                "img_id": 115,
                "product_id": 14,
                "img_url": {
                    "url": "http://cf.yxadult.xyz/images/20191222/48b58d621696047eb41ffbf8541f8d81.jpg",
                    "create_time": "2019-12-22 16:13:06"
                }
            }
        ],
        "main_imgs": [
            {
                "id": 50,
                "img_id": 118,
                "product_id": 14,
                "img_url": {
                    "url": "http://cf.yxadult.xyz/images/20191222/6d0a7c23bb2ca38e0e284f08b212ac3b.jpg",
                    "create_time": "2019-12-22 16:13:21"
                }
            },
            {
                "id": 51,
                "img_id": 119,
                "product_id": 14,
                "img_url": {
                    "url": "http://cf.yxadult.xyz/images/20191222/7feb22867996c5ebbbb135d298d3550c.jpg",
                    "create_time": "2019-12-22 16:13:26"
                }
            }
        ]
    },
]
```

