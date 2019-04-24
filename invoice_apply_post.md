# 提交发票申请

## 说明

|  Auth  |  Method  |  url  |
| :----  | :----:   | :---- |
|  Login  |  POST  |  /invoice/apply  |

## 请求参数

|  参数  |  类型  |  是否必选  |  说明  |
| :---- | :----: | :----:   | :----  |
| phone | string | 1 | 手机号码 |
| danWeiName | string | 1 | 单位名称 |
| invoiceType | int | 0 | 发票类型(0:普票, 1:专票), 默认0 |
| invoiceTitle | string | 1 | 发票抬头 |
| taxNum | string | 1 | 税号 |
| bank | string | 1 | 开户银行, |
| bankAccount | string | 1 | 开户银行账号 |

## 响应参数

> 除非另外说明，否则响应字段的意思请 refer [invoice_apply_spec.md](/invoice_apply_spec.md) 中同名字段

|  参数  |  类型  |  是否必选  |  说明  |
| :---- | :----: | :----:   | :----  |
|  id  |  int  |  1  |  |
|  createDt  |  string  |  1  |  |
|  uid  |  int  |  1  |  |
|  phone  |  string  |  1  |  |
|  business  |  string  |  0  |  |
|  bid  |  int  |  0  |  |
|  danWeiName  |  string  |  1  |  |
|  invoiceType  |  int  |  1  |  |
|  invoiceTitle  |  string  |  1  |  |
|  taxNum  |  string  |  1  |  |
|  bank  |  string  |  1  |  |
|  bankAccount  |  string  |  1  |  |
|  kaiFaPiaoDt  |  string  |  0  |  |

## 请求示例

```
{
    "phone": "15623967785",
    "danWeiName": "xxx",
    "danWeiAddr": "yyy",
    "invoiceType": 0,
    "invoiceTitle": "hello",
    "taxNum": "123",
    "bank": "中国银行",
    "bankAccount": "456"
}
```

## 响应示例

```
{
    "code": 200,
    "data": {
        "createDt": "2019-04-24 20:46:29",
        "uid": 1,
        "phone": "15623967785",
        "business": "",
        "bid": 0,
        "invoiceType": 0,
        "danWeiName": "xxx",
        "invoiceTitle": "hello",
        "taxNum": "123",
        "bank": "中国银行",
        "bankAccount": "456",
        "id": "2"
    }
}
```