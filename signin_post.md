# 提交签到数据

## 说明

|  Auth  |  Method  |  url  |
| :----  | :----:   | :---- |
|  NONE  |  POST  |  /signin  |

## 请求参数

|  参数  |  类型  |  是否必选  |  说明  |
| :---- | :----: | :----:   | :----  |
| class | int | 1 | 班级id |
| phone | string | 1 | 手机号码 |
| name | string | 1 | 姓名 |
| gender | int | 1 | 性别(1:男, 2:女) |
| danWeiName | string | 0 | 单位名称 |

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
    "danWeiName": "xxx"
}
```

## 响应示例

```
{
    "code": 200,
    "msg": "success"
}
```