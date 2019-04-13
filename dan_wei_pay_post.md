# 提交单位缴费订单

## 说明

|  Auth  |  Method  |  url  |
| :----  | :----:   | :---- |
|  NONE  |  POST  |  /danweipay  |

## 请求参数

|  参数  |  类型  |  是否必选  |  说明  |
| :---- | :----: | :----:   | :----  |
| class | int | 1 | 班级id |
| phone | string | 1 | 手机号码 |
| name | string | 1 | 单位名称 |
| studentCnt | int | 1 | 学员人数 |
| stayCnt | int | 0 | 住宿人数 |

## 响应参数

|  参数  |  类型  |  是否必选  |  说明  |
| :---- | :----: | :----:   | :----  |

## 请求示例

```
{
    "class": 2,
    "phone": "15623967785",
    "name": "xxx单位",
    "studentCnt": 2,
    "stayCnt": 1
}
```

## 响应示例

```
{
    "code": 200,
    "msg": "success"
}
```