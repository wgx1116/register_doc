# 支付订单信息字段说明

|  参数  |  类型  |  说明  |
| :---- | :----: | :----  |
|  id  |  int  |  id  |
|  orderNo  |  string  |  支付订单号,专门用于支付,给到支付宝或者微信支付等支付商  |
|  createDt  |  string  |  创建时间  |
|  phone  |  string  |  用户手机号码,用来标志用户,冗余字段,方便查询  |
|  business  |  string  |  业务  |
|  bid  |  int  |  和业务对应的id  |
|  amount  |  float  |  支付订单金额  |
|  payType  |  string  |  支付类型(alipay:支付宝支付, wxpay:微信支付)  |
|  payFirstNotifyDt  |  string  |  第1次收到支付回调通知时间  |
|  payFirstLog  |  string  |  json格式,记录第1次收到支付回调通知信息的快照  |
|  paySuccessDt  |  string  |  我方成功处理支付回调通知的时间  |
|  payDt  |  string  |  用户支付时间  |
|  payAmount  |  string  |  用户支付金额  |
|  payTradeNo  |  string  |  支付交易号,一般退款的时候需要用到  |
|  payLog  |  string  |  json格式,记录支付回调通知信息的快照  |
|  refundRequestDt  |  string  |  发起退款时间  |
|  refundDoneDt  |  string  |  退款完成时间  |
|  refundLog  |  string  |  json格式,记录退款完成通知信息的快照  |

