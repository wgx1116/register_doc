# 我的报名记录数据

## 说明

|  Auth  |  Method  |  url  |
| :----  | :----:   | :---- |
|  Login  |  GET  |  /me/reg/listdata  |

## 请求参数

|  参数  |  类型  |  是否必选  |  说明  |
| :---- | :----: | :----:   | :----  |
| page | int | 0 | 分页,page,从0开始,默认0 |
| limit | int | 0 | 分页,limit,默认10 |

## 响应参数

> * 除非另外说明，否则响应字段 list 中的字段的意思请 refer [reglog_spec.md](/reglog_spec.md) 中同名字段

|  参数  |  类型  |  是否必选  |  说明  |
| :---- | :----: | :----:   | :----  |
| total | int | 1 | 总条数 |
|  list  |  object array  |  1  | 我的报名记录 |


## 请求示例

```

```

## 响应示例

```

```