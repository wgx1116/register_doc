# 提交单位缴费订单

## 说明

|  Auth  |  Method  |  url  |
| :----  | :----:   | :---- |
|  Login  |  POST  |  /danweipay  |

## 请求参数

|  参数  |  类型  |  是否必选  |  说明  |
| :---- | :----: | :----:   | :----  |
| class | int | 1 | 班级id |
| danWeiName | string | 1 | 单位名称 |
| contactName | string | 1 | 联系人名称 |
| contactPhone | string | 1 | 联系人电话号码 |
| studentCnt | int | 1 | 学员人数 |
| stayCnt | int | 0 | 住宿人数 |

## 响应参数

> 除非另外说明，否则响应字段的意思请 refer [dan_wei_pay_spec.md](/dan_wei_pay_spec.md) 中同名字段

|  参数  |  类型  |  是否必选  |  说明  |
| :---- | :----: | :----:   | :----  |
|  id  |  int  |  1  |  |
|  createDt  |  string  |  1  |  |
|  token  |  string  |  1  |  |
|  classId  |  int  |  1  |  |
|  uid  |  int  |  1  |  |
|  danWeiName  |  string  |  1  |  |
|  contactName  |  string  |  1  |  |
|  contactPhone  |  string  |  1  |  |
|  studentCnt  |  int  |  1  |  |
|  stayCnt  |  int  |  1  |  |
|  totalFee  |  float  |  1  |  |
|  payMoney  |  float  |  1  |  |

## 请求示例

```
{
    "class": 20,
    "danWeiName": "xxx单位",
    "contactName": "15623967785",
    "contactPhone": "15623967785",
    "studentCnt": 10,
    "stayCnt": 2
}
```

## 响应示例

```
{
    "code": 200,
    "data": {
        "createDt": "2019-04-25 22:47:51",
        "token": "5QG0DZ4X47",
        "classId": 20,
        "uid": 1,
        "danWeiName": "xxx单位",
        "contactName": "15623967785",
        "contactPhone": "15623967785",
        "studentCnt": 10,
        "stayCnt": 2,
        "totalFee": 1,
        "payMoney": 0,
        "id": "10"
    }
}
```