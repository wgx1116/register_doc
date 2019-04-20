# 提交报名数据

## 说明

|  Auth  |  Method  |  url  |
| :----  | :----:   | :---- |
|  Login  |  POST  |  /reg  |

## 请求参数

|  参数  |  类型  |  是否必选  |  说明  |
| :---- | :----: | :----:   | :----  |
| class | int | 1 | 班级id |
| name | string | 1 | 姓名 |
| gender | int | 1 | 性别(1:男, 2:女) |
| phone | string | 1 | 手机号码 |
| zhiWu | string | 0 | 职务 |
| zhuSu | 0-1 | 1 | 是否住宿(0:否, 1:是) |
| danWeiName | string | 1 | 单位名称 |
| danWeiAddr | string | 0 | 单位地址 |
| invoice | 0-1 | 1 | 是否要发票(0:否, 1:是) |
| invoiceType | int | 0 | 发票类型(0:普票, 1:专票), invoice=1 时必选 |
| invoiceTitle | string | 0 | 发票抬头, invoice=1 时必选 |
| taxNum | string | 0 | 税号, invoice=1 时必选 |
| bank | string | 0 | 开户银行, invoice=1 时必选 |
| bankAccount | string | 0 | 开户银行账号, invoice=1 时必选 |
| zhiCheng | string | 0 | 职称 |

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
    "class": 2,
    "name": "汪国新",
    "gender": 1,
    "phone": "15623967785",
    "zhiWu": "",
    "zhuSu": 0,
    "danWeiName": "xxx",
    "danWeiAddr": "yyy",
    "invoice": 0,
    "invoiceType": 0,
    "invoiceTitle": "",
    "taxNum": "",
    "bank": "",
    "bankAccount": "",
    "zhiCheng": ""
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
        "name": "汪国新",
        "gender": "1",
        "phone": "15623967785",
        "zhuSu": "0",
        "zhiWu": "",
        "danWeiName": "xxx",
        "danWeiAddr": "yyy",
        "invoice": "0",
        "invoiceType": "0",
        "invoiceTitle": null,
        "taxNum": null,
        "bank": null,
        "bankAccount": null,
        "zhiCheng": "",
        "totalFee": "0.00",
        "payMoney": "0.00"
    }
}
```