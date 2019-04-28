# ReadMe

接口文档

# Some Route

|  Auth  |  Method  |  url  |  说明  |
| :----  | :----:   | :---- | :---- |
|  NONE  |  GET  |  /  |  首页 `index.html.php`  |
|  NONE  |  POST  |  /login/sendphonecode  |  refer [login_sendphonecode.md](/login_sendphonecode.md)  |
|  NONE  |  GET  |  /login  |  登录页 `login.html.php`  |
|  NONE  |  POST  |  /login  |  refer [login_post.md](/login_post.md)  |
|  Login  |  DELETE  |  /logout  |  退出  |
|  Login  |  GET  |  /me  |  我的 页 `me.html.php`  |
|  Login  |  GET  |  /me/reg/list  |  我的报名记录 页 `my_register_list.html.php`  |
|  Login  |  GET  |  /me/reg/listdata  |  refer [my_reg_listdata.md](/my_reg_listdata.md)  |
|  Login  |  GET  |  /me/signin/list  |  我的签到记录 页 `my_signin_list.html.php`  |
|  Login  |  GET  |  /me/signin/listdata  |  refer [my_signin_listdata.md](/my_signin_listdata.md)  |
|  Login  |  GET  |  /me/payorder/list  |  我的缴费记录 页 `my_payorder_list.html.php`  |
|  Login  |  GET  |  /me/payorder/listdata  |  refer [my_payorder_listdata.md](/my_payorder_listdata.md)  |
|  Login  |  GET  |  /pay  |  refer [pay.md](/pay.md)  |
|  Login  |  GET  |  /pay/result  |  refer [pay_result.md](/pay_result.md)  |
|  Login  |  GET  |  /reg  |  报名登记页 `register.html.php` |
|  Login  |  POST  |  /reg  |  refer [reg_post.md](/reg_post.md)  |
|  Login  |  GET  |  /reg/detail  |  refer [reg_detail.md](/reg_detail.md)  |
|  Login  |  POST  |  /reg/pay/dwptoken  |  refer [reg_pay_dwp_token.md](/reg_pay_dwp_token.md)  |
|  Login  |  GET  |  /danweipay  |  单位缴费页 `dwp.html.php`  |
|  Login  |  POST  |  /danweipay  |  refer [dan_wei_pay_post.md](/dan_wei_pay_post.md)  |
|  Login  |  GET  |  /danweipay/detail  |  refer [dan_wei_pay_detail.md](/dan_wei_pay_detail.md)  |
|  Login  |  GET  |  /signin  |  签到页 `signin.html.php`  |
|  Login  |  POST  |  /signin  |  refer [signin_post.md](/signin_post.md)  |
|  Login  |  GET  |  /signin/detail  |  签到详情页,Query Parameter(id:签到id) `signin_detail.html.php`  |
|  Login  |  GET  |  /invoice/apply  |  发票申请页 `invoice_apply.html.php`  |
|  Login  |  POST  |  /invoice/apply  |  refer [invoice_apply_post.md](/invoice_apply_post.md)  |
|  Login  |  GET  |  /invoice/apply/detail  |  refer [invoice_apply_detail.md](/invoice_apply_detail.md)  |

# Index

|  文档  |  说明  |
| :---- | :----  |
| [api_specification.md](/api_specification.md) | 接口规范 |
| [template.md](/template.md) | 接口文档模板 |
| [pay_order_spec.md](/pay_order_spec.md) | 支付订单信息字段说明 |
| [pay.md](/pay.md) | 发起支付 |
| [pay_result.md](/pay_result.md) | 支付结果 |
| [login_sendphonecode.md](/login_sendphonecode.md) | 发送登录手机短信验证码 |
| [login_post.md](/login_post.md) | 登录 |
| [my_reg_listdata.md](/my_reg_listdata.md) | 我的报名记录数据 |
| [my_signin_listdata.md](/my_signin_listdata.md) | 我的签到记录数据 |
| [my_payorder_listdata.md](/my_payorder_listdata.md) | 我的缴费记录数据 |
| [class_spec.md](/class_spec.md) | 班级信息字段说明 |
| [reglog_spec.md](/reglog_spec.md) | 报名信息字段说明 |
| [reg_post.md](/reg_post.md) | 提交报名数据 |
| [reg_detail.md](/reg_detail.md) | 报名详情页 |
| [reg_pay_dwp_token.md](/reg_pay_dwp_token.md) | 使用单位缴费凭证支付 |
| [dan_wei_pay_spec.md](/dan_wei_pay_spec.md) | 单位缴费信息字段说明 |
| [dan_wei_pay_post.md](/dan_wei_pay_post.md) | 提交单位缴费订单 |
| [dan_wei_pay_detail.md](/dan_wei_pay_detail.md) | 单位缴费详情页 |
| [signin_spec.md](/signin_spec.md) | 签到信息字段说明 |
| [signin_post.md](/signin_post.md) | 提交签到数据 |
| [invoice_apply_spec.md](/invoice_apply_spec.md) | 发票申请信息字段说明 |
| [invoice_apply_post.md](/invoice_apply_post.md) | 提交发票申请 |
| [invoice_apply_detail.md](/invoice_apply_detail.md) | 发票申请详情页 |
