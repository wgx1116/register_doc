# 提交签到数据

## 说明

|  Auth  |  Method  |  url  |
| :----  | :----:   | :---- |
|  NONE  |  POST  |  /signin  |

## 请求参数

|  参数  |  类型  |  是否必选  |  说明  |
| :---- | :----: | :----:   | :----  |
| name | string | 1 | 姓名 |
| gender | int | 1 | 性别(1:男, 2:女) |
| phone | string | 1 | 手机号码 |
| danWeiName | string | 0 | 单位名称 |
| banCi | string | 1 | 班次 |
| isPay | 0-1 | 1 | 是否已缴费(0:否, 1:是) |
| payToken | string | 0 | 缴费票据 |

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