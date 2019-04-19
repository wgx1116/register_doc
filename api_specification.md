# 接口规范

## 请求约定

* 使用 `http` 协议请求服务器
* 除非另外说明，使用 `application/x-www-form-urlencoded` 或者 `application/json` 向服务器提交数据
* 尽量使用驼峰写法向服务器提交数据
* 如果接口需要分页，约定分页参数为 `limit,page`, limit 表示每页返回的数据条数, page 表示页数, limit 默认值 20, page 从 0 开始，默认值 0。

## 响应约定

* 除非另外说明，正常情况下服务器使用 `application/json` 返回响应数据
* 尽量使用驼峰写法返回响应数据
* 除非另外说明，Response Status Code = 200, 正常
* 除非另外说明，Response Status Code >= 400, 出错了。出错时，如果服务器使用 `application/json` 返回响应数据，那么需要返回 `msg` 字段表示出错的原因；否则认为服务器错误
* Response Status Code == 430, 请登录
* Response Status Code == 431, 请选择班级
* Response Status Code == 440, 给 {{phone}} 发送 {{type}} 类型的短信已超过今天的限制