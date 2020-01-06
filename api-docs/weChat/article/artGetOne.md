## 查看文章详情 /wechat/article/artGetOne

- **`HTTPS 请求方式`** GET

## Example Request
```
https://{host}/api/v1/article/${:id}

## Request Parameter

| 参数名       | 必选   | 参数对应值 | 说明                  |
| ------------ | ------ | ---------- | --------------------|



## Request Body

## Response Parameter

| 参数名              | 必选   | 参数对应值 | 说明                              |
| ------------------- | ------ | ---------- | --------------------------------|
| id                  | `true` | `int    `  | 主键id                          |
| title               | `true` | `string`   | 文章标题                         |
| like_num            | `true` | `int`      | 点赞数                           |
| content             | `true` | `string`   | 文章内容                         |
| status              | `true` | `int`      | 文章的状态，0是正常               |
| read_num            | `true` | `int`      | 阅读数                           |
| create_time         | `true` | `string`   | 创建时间                         |
| comment             | `true` | `string`   | 评论                             |
| user_id             | `true` | `string`   | 用户id                           |
| article_id          | `true` | `string`   | 文章id                           |
| content             | `true` | `string`   | 评论内容                         |
| create_time         | `true` | `string`   | 评论创建时间                     |

## Response Body

```
{
    "id": 3,
    "title": "我的模板",
    "content": "<p>1<img src=\"/ueditor/php/upload/image/20200106/1578300714287039.jpg\" title=\"1578300714287039.jpg\" alt=\"u=2229864841,4232235061&amp;fm=26&amp;gp=0.jpg\"/></p>",
    "like_num": 123,
    "status": 0,
    "read_num": 1231,
    "create_time": "2020-01-06 16:52:01",
    "comment": [
        {
            "id": 2,
            "user_id": 49,
            "article_id": 3,
            "content": "真好",
            "create_time": "2020-01-06 16:55:25"
        },
        {
            "id": 2,
            "user_id": 49,
            "article_id": 3,
            "content": "真好",
            "create_time": "2020-01-06 16:55:25"
        }
    ]
}


comment可能为空;
    "comment":[]
```

