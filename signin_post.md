# 提交签到数据

## 说明

|  Auth  |  Method  |  url  |
| :----  | :----:   | :---- |
|  Login  |  POST  |  /signin  |

## 请求参数

|  参数  |  类型  |  是否必选  |  说明  |
| :---- | :----: | :----:   | :----  |
| class | int | 1 | 班级id |
| phone | string | 1 | 手机号码 |
| name | string | 1 | 姓名 |
| gender | int | 1 | 性别(1:男, 2:女) |
| danWeiName | string | 0 | 单位名称 |

## 响应参数

> 除非另外说明，否则响应字段的意思请 refer [signin_spec.md](/signin_spec.md) 中同名字段

|  参数  |  类型  |  是否必选  |  说明  |
| :---- | :----: | :----:   | :----  |
|  id  |  int  |  1  |  |
|  createDt  |  string  |  1  |  |
|  classId  |  int  |  1  |  |
|  uid  |  int  |  1  |  |
|  name  |  string  |  1  |  |
|  gender  |  int  |  1  |  |
|  phone  |  string  |  1  |  |
|  danWeiName  |  string  |  1  |  |
|  faZiLiaoDt  |  string  |  0  |  |

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
    "data": {
        "createDt": "2019-04-24 16:39:23",
        "classId": 2,
        "uid": 1,
        "name": "汪国新",
        "gender": 1,
        "phone": "15623967785",
        "danWeiName": "xxx",
        "id": "13"
    }
}
```