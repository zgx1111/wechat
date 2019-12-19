## 获得首页10个商品分类 /wechat/category/home/

- **`HTTPS 请求方式`** GET

## Example Request
```
https://yxadult.xyz/api/v1/category/home
```

## Request Parameter

| 参数名       | 必选   | 参数对应值 | 说明                  |
| ------------ | ------ | ---------- | --------------------|



## Request Body


## Response Parameter

| 参数名              | 必选   | 参数对应值 | 说明                              |
| ------------------- | ------ | ---------- | --------------------------------|
| id                  | `true` | `int    `  | 主键id                          |
| name                | `true` | `string`   | 分类名字                         |
| topic_img_id        | `true` | `int`      | 主图id                           |
| update_time         | `true` | `int`      | 更新时间                         |
| img                 | `true` | `array`    | 图片信息                         |


## Response Body

```
返回8个分类

[
    {
        "id": 1,
        "name": "男性用品",
        "topic_img_id": 172,
        "description": null,
        "update_time": "2019-12-01 12:30:51",
        "img": {
            "url": "http://z.cn/images/20191201/09f2bddc368dc868e38f9a52b64cbca6.jpg",
            "create_time": "2019-12-01 12:30:51"
        }
    },
    {
        "id": 2,
        "name": "女性用品",
        "topic_img_id": 181,
        "description": null,
        "update_time": "2019-12-01 18:23:20",
        "img": {
            "url": "http://z.cn/images/20191201/b328488d136cb2815e6d3228d516dbbb.jpg",
            "create_time": "2019-12-01 18:23:20"
        }
    },
    ...
]
```

