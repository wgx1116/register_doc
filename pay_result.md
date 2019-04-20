# 支付结果

## 说明

|  Auth  |  Method  |  url  |
| :----  | :----:   | :---- |
|  Login  |  GET  |  /pay/result  |

## 请求参数

|  参数  |  类型  |  是否必选  |  说明  |
| :---- | :----: | :----:   | :----  |
| id | string | 1 | 支付订单id |

## 响应参数

> 除非另外说明，否则响应字段 payOrder 中的字段的意思请 refer [pay_order_spec.md](/pay_order_spec.md) 中同名字段

|  参数  |  类型  |  是否必选  |  说明  |
| :---- | :----: | :----:   | :----  |
| success | 0-1 | 1 | 是否成功(0:否, 1:是) |
| payOrder | object | 1 | 支付订单 |


## 请求示例

```
GET /pay/result?id=5
```

## 响应示例

```
{
    "code": 200,
    "data": {
        "success": 0,
        "payOrder": {
            "id": "5",
            "createDt": "2019-04-20 18:06:35",
            "uid": "1",
            "business": "register",
            "bid": "20",
            "amount": "0.01",
            "payType": "wxpay",
            "payFirstNotifyDt": null,
            "paySuccessDt": null,
            "payDt": null,
            "refundRequestDt": null,
            "refundDoneDt": null
        }
    }
}
```