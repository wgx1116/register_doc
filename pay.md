# 发起支付

## 说明

|  Auth  |  Method  |  url  |
| :----  | :----:   | :---- |
|  Login  |  GET  |  /pay  |

## 请求参数

|  参数  |  类型  |  是否必选  |  说明  |
| :---- | :----: | :----:   | :----  |
| paytype | string | 0 | 支付类型(alipay:支付宝支付, wxpay:微信支付) 默认 alipay |
| business | string | 1 | 业务(register:报名登记) |
| bid | string | 0 | 业务对应的id, () 不用传 |
| amount | float | 0 | 金额, (register) 不用传 |


## 响应参数

> 除非另外说明，否则响应字段 payOrder 中的字段的意思请 refer [pay_order_spec.md](/pay_order_spec.md) 中同名字段

|  参数  |  类型  |  是否必选  |  说明  |
| :---- | :----: | :----:   | :----  |
| timeExpire | int | 1 | 过期时间，时间戳 |
| qrCode | int | 1 | 支付二维码url |
| payOrder | object | 1 | 支付订单 |


## 请求示例

```
GET /pay?paytype=wxpay&business=register&bid=20
```

## 响应示例

```
{
    "code": 200,
    "data": {
        "timeExpire": 1555761995,
        "qrCode": "weixin://wxpay/bizpayurl?pr=XBdZpSH",
        "payOrder": {
            "createDt": "2019-04-20 18:06:35",
            "uid": 1,
            "business": "register",
            "bid": 20,
            "amount": 0.01,
            "payType": "wxpay",
            "id": "5"
        }
    }
}
```