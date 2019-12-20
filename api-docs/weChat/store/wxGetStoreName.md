## 查看门店名字 /wechat/store/wxGetStoreName/

- **`HTTPS 请求方式`** POST

## Example Request
```
https://{host}/api/v1/storewxGetStoreName
```

## Request Parameter

| 参数名       | 必选   | 参数对应值 | 说明                  |
| ------------ | ------ | ---------- | --------------------|
| id           | `true` | `int`      | 门店id               |


## Request Body

```
{
    "id":1
}
```



## Response Parameter

| 参数名              | 必选   | 参数对应值 | 说明                               |
| ------------------- | ------ | ---------- | ---------------------------------|
| status              | `true` | `Boolean`  | 返回状态                          |
| name                | `true` | `string`   | 门店名字                          |


## Response Body

```
门店存在:
{
    "status": true,
    "name": "如佳情侣主题酒店"
}


门店不存在：
{
    "status": false,
    "name": null
}
```

