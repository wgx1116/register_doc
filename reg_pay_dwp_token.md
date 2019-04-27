# 使用单位缴费凭证支付

## 说明

|  Auth  |  Method  |  url  |
| :----  | :----:   | :---- |
|  Login  |  POST  |  /reg/pay/dwptoken  |

## 请求参数

|  参数  |  类型  |  是否必选  |  说明  |
| :---- | :----: | :----:   | :----  |
| id | int | 1 | 报名id |
| token | string | 1 | 单位缴费凭证 |

## 响应参数

> 除非另外说明，否则响应字段的意思请 refer [reglog_spec.md](/reglog_spec.md) 中同名字段

|  参数  |  类型  |  是否必选  |  说明  |
| :---- | :----: | :----:   | :----  |
|  id  |  int  |  1  |  |
|  createDt  |  string  |  1  |  |
|  classId  |  int  |  1  |  |
|  uid  |  int  |  1  |  |
|  name  |  string  |  1  |  |
|  gender  |  int  |  1  |  |
|  avatar  |  string  |  0  |  |
|  phone  |  string  |  1  |  |
|  email  |  string  |  0  |  |
|  addr  |  string  |  0  |  |
|  zhuSu  |  0-1  |  1  |  |
|  buMen  |  string  |  0  |  |
|  zhiWu  |  string  |  0  |  |
|  danWeiName  |  string  |  1  |  |
|  danWeiAddr  |  string  |  0  |  |
|  invoice  |  0-1  |  1  |  |
|  invoiceType  |  int  |  0  |  |
|  invoiceTitle  |  string  |  0  |  |
|  taxNum  |  string  |  0  |  |
|  bank  |  string  |  0  |  |
|  bankAccount  |  string  |  0  |  |
|  zhiCheng  |  string  |  0  |  |
|  totalFee  |  float  |  1  |  |
|  payMoney  |  float  |  1  |  |

## 请求示例

```
{
    "id": 13,
    "token": "YOZVFZW5Y9"
}
```

## 响应示例

```
{
    "code": 200,
    "data": {
        "id": "13",
        "createDt": "2019-04-19 23:26:58",
        "classId": "2",
        "uid": "1",
        "name": "汪汪",
        "gender": "1",
        "phone": "15623967785",
        "zhuSu": "1",
        "zhiWu": "php开发",
        "danWeiName": "fuck",
        "danWeiAddr": "yyy",
        "zhiCheng": "",
        "totalFee": "0.01",
        "payMoney": 0.01,
        "dwpId": 40,
        "dwpPayDt": "2019-04-28 00:06:48"
    }
}
```