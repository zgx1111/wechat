## 增加评论 /wechat/article/commentAdd

- **`HTTPS 请求方式`** POST

## Example Request
```
https://{host}/api/v1/comment/commentAdd
```

## Request Parameter

| 参数名       | 必选   | 参数对应值 | 说明                  |
| ------------ | ------ | ---------- | --------------------|
| id           | `true` | `int`      | 文章id               |
| content      | `true` | `string`   | 评论内容             |


## Request Body

用户token令牌在header里传
{
    "id":8,
    "content":"wewqewqe"
}

## Response Parameter

| 参数名              | 必选   | 参数对应值 | 说明                              |
| ------------------- | ------ | ---------- | --------------------------------|
| status              | `true` | `string `  | 返回状态                         |



## Response Body

```
成功：
{
    "status": true,
}

失败：
{
    "status":false,
}
```

