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
    "id": 337,
    "name": "梨花带雨1个",
    "price": "123.00",
    "cost": "22.00",
    "stock": 123,
    "sales":0,
    "state": 1,
    "delete_time": null,
    "category_id": 1,
    "main_img_url": "http://yxadult.xyz/images",
    "create_time": "2019-12-19 14:16:16",
    "update_time": "2019-12-19 14:20:13",
    "summary": "123",
    "img_id": null,
    "storehouse_id": 6,
    "imgs": [
        {
            "id": 1110,
            "img_id": 1645,
            "product_id": 337,
            "img_url": {
                "url": "http://z.cn/images/20191219/118cd7ab22aae6deaa9d34ce395ba950.jpg",
                "create_time": "2019-12-19 14:16:14"
            }
        },
        {
            "id": 1111,
            "img_id": 1646,
            "product_id": 337,
            "img_url": {
                "url": "http://z.cn/images/20191219/01a62a3117d4568fa21e51beac4e93b9.jpg",
                "create_time": "2019-12-19 14:16:31"
            }
        }
    ],
    "main_imgs": [
        {
            "id": 47,
            "img_id": 1643,
            "product_id": 337,
            "img_url": {
                "url": "http://z.cn/images/20191219/ab9d8ba0a98a0a03369006091fc433b4.jpg",
                "create_time": "2019-12-19 14:16:07"
            }
        }
    ]
}
```

