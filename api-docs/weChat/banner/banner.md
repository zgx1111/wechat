## 获得轮播图 /wechat/banner/banner/

- **`HTTPS 请求方式`** GET

## Example Request
```
https://yxadult.xyz/api/v1/banner/1
```

## Request Parameter

| 参数名       | 必选   | 参数对应值 | 说明                  |
| ------------ | ------ | ---------- | --------------------|
| id           | `true` | `int   `   | 轮播主键id           |


## Request Body

```

```



## Response Parameter

| 参数名              | 必选   | 参数对应值 | 说明                               |
| ------------------- | ------ | ---------- | ---------------------------------|
| id                  | `true` | `int`      | 主键ID                            |
| name                | `true` | `string`   | 名字                              |
| description         | `true` | `string`   | 简述                              |
| items               | `true` | `int`      | 轮播图片                          |

## Response Body

```
{
    "id": 1,
    "name": "首页置顶",
    "description": "首页轮播图",
    "items": [
        {
            "id": 1,
            "type": 1,
            "create_time": "1970-01-01 08:00:00",
            "img": {
                "url": "https://yxadult.xyz/images/20191217/dba532443cf12d032855e512d5c35466.jpg",
                "create_time": "2019-12-17 12:05:23"
            }
        },
        {
            "id": 2,
            "type": 1,
            "create_time": "1970-01-01 08:00:00",
            "img": {
                "url": "https://yxadult.xyz/images/20191217/a3014b0526fb527f3342c9c777800dd4.jpg",
                "create_time": "2019-12-17 12:05:54"
            }
        },
        {
            "id": 3,
            "type": 1,
            "create_time": "1970-01-01 08:00:00",
            "img": {
                "url": "https://yxadult.xyz/images/20191217/4714e4dbabd3ff64fee988dd5d29a010.jpg",
                "create_time": "2019-12-17 12:05:42"
            }
        },
        {
            "id": 5,
            "type": 1,
            "create_time": "1970-01-01 08:00:00",
            "img": {
                "url": "https://yxadult.xyz/images/20191217/8b44cd4c56e29ffc28f0e85a17a831cd.jpg",
                "create_time": "2019-12-17 12:06:08"
            }
        }
    ]
}
```

