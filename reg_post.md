# 提交报名数据

## 说明

|  Auth  |  Method  |  url  |
| :----  | :----:   | :---- |
|  NONE  |  POST  |  /reg  |

## 请求参数

|  参数  |  类型  |  是否必选  |  说明  |
| :---- | :----: | :----:   | :----  |
| class | int | 1 | 班级id |
| phone | string | 1 | 手机号码 |
| name | string | 1 | 姓名 |
| gender | int | 1 | 性别(1:男, 2:女) |
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

|  参数  |  类型  |  是否必选  |  说明  |
| :---- | :----: | :----:   | :----  |

## 请求示例

```
{
    "class": 2,
    "phone": "15623967785",
    "name": "汪国新",
    "gender": 1,
    "zhiWu": "",
    "zhuSu": 0,
    "danWeiName": "xxx",
    "danWeiAddr": "",
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
    "msg": "success"
}
```