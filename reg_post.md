# 提交报名数据

## 说明

|  Auth  |  Method  |  url  |
| :----  | :----:   | :---- |
|  NONE  |  POST  |  /reg  |

## 请求参数

|  参数  |  类型  |  是否必选  |  说明  |
| :---- | :----: | :----:   | :----  |
| class | int | 0 | 班级id |
| phone | string | 1 | 手机号码 |
| name | string | 1 | 姓名 |
| gender | int | 1 | 性别(1:男, 2:女) |
| addr | string | 1 | 地址 |
| buMen | string | 1 | 部门 |
| zhiWu | string | 1 | 职务 |
| zhuSu | 0-1 | 1 | 是否住宿(0:否, 1:是) |
| danWeiName | string | 0 | 单位名称 |
| danWeiAddr | string | 0 | 单位地址 |
| invoice | 0-1 | 1 | 是否要发票(0:否, 1:是) |
| invoiceTitle | string | 0 | 发票抬头 |
| invoiceType | int | 0 | 发票类型(0:普票, 1:专票) |
| taxNum | string | 1 | 税号 |
| bank | string | 1 | 开户银行 |
| bankAccount | string | 1 | 开户银行账号 |
| zhiCheng | string | 1 | 职称 |

## 响应参数

|  参数  |  类型  |  是否必选  |  说明  |
| :---- | :----: | :----:   | :----  |

## 请求示例

```
```

## 响应示例

```
{
    "code": 200,
    "msg": "success"
}
```