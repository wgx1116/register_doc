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

> 除非另外说明，否则响应字段的意思请 refer [pay_order_spec.md](/pay_order_spec.md) 中同名字段

|  参数  |  类型  |  是否必选  |  说明  |
| :---- | :----: | :----:   | :----  |
|  id  |  int  |  1  |  |
|  createDt  |  string  |  1  |  |
|  uid  |  1  |  1  |  |
|  business  |  string  |  1  |  |
|  bid  |  int  |  1  |  |
|  amount  |  float  |  1  |  |
|  payType  |  string  |  1  |  |
|  qrCodeUrl  |  string  |  1  |  |
|  prePayExpireDt  |  string  |  1  |  |
|  payFirstNotifyDt  |  string  |  0  |  |
|  paySuccessDt  |  string  |  1  |  |
|  payDt  |  string  |  1  |  |
|  refundRequestDt  |  string  |  0  |  |
|  refundDoneDt  |  string  |  0  |  |


## 请求示例

```
GET /pay?paytype=wxpay&business=register&bid=16
```

## 响应示例

```
{
    "code": 200,
    "data": {
        "id": "6",
        "createDt": "2019-04-22 11:59:31",
        "uid": "1",
        "business": "register",
        "bid": "16",
        "amount": "0.01",
        "payType": "wxpay",
        "qrCodeUrl": "weixin://wxpay/bizpayurl?pr=6NgT89j",
        "prePayExpireDt": "2019-04-22 14:04:47",
        "payFirstNotifyDt": null,
        "paySuccessDt": null,
        "payDt": null,
        "refundRequestDt": null,
        "refundDoneDt": null
    }
}
```