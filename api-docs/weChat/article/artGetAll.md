## 查看所有文章 /wechat/article/artGetAll

- **`HTTPS 请求方式`** GET

## Example Request
```
https://{host}/api/v1/article/artGetAll
```

## Request Parameter

| 参数名       | 必选   | 参数对应值 | 说明                  |
| ------------ | ------ | ---------- | --------------------|



## Request Body

## Response Parameter

| 参数名              | 必选   | 参数对应值 | 说明                              |
| ------------------- | ------ | ---------- | --------------------------------|
| status              | `true` | `string `  | 返回状态                         |
| id                  | `true` | `int    `  | 主键id                          |
| title               | `true` | `string`   | 文章标题                         |
| like_num            | `true` | `int`      | 点赞数                           |
| status              | `true` | `int`      | 文章的状态，0是正常               |
| read_num            | `true` | `int`      | 阅读数                           |
| create_time         | `true` | `string`   | 创建时间                         |


## Response Body

```
{
    "status": true,
    "art": [
        {
            "id": 3,
            "title": "啊啊啊1",
            "like_num": 23111,
            "status": 0,
            "read_num": 213,
            "create_time": "2020-01-03 17:41:28"
        },
        {
            "id": 4,
            "title": "dsf",
            "like_num": 231,
            "status": 127,
            "read_num": 213,
            "create_time": "2020-01-03 17:44:44"
        }
    ]
}
```

