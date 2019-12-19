## 获得一个分类的信息 /wechat/category/one/

- **`HTTPS 请求方式`** GET

## Example Request
```
https://{host}/api/v1/category/one
```

## Request Parameter

| 参数名       | 必选   | 参数对应值 | 说明                  |
| ------------ | ------ | ---------- | --------------------|
| category_id  | `true` | `int`      | 分类id              |



## Request Body

```
{
    "category_id":1
}

```
## Response Parameter

| 参数名              | 必选   | 参数对应值 | 说明                              |
| ------------------- | ------ | ---------- | --------------------------------|
| id                  | `true` | `int    `  | 主键id                          |
| name                | `true` | `string`   | 分类名字                         |
| topic_img_id        | `true` | `int`      | 主图id                          |
| update_time         | `true` | `int`      | 更新时间                         |
| description         | `true` | `string`   | 描述信息                         |


## Response Body

```

    {
        "id": 2,
        "name": "女性用品",
        "topic_img_id": 181,
        "description": null,
        "update_time": "2019-12-01 18:23:20"
    }

```

