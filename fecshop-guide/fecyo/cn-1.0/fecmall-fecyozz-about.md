Fecyozz 子账户扩展-简介
============


### 子账户扩展需求

一：账户体系

1.总账户可以在商城`直接注册`，`手机号注册`（需要验证码验证），注册后是`未激活`状态，需要后台进行`审核`

2.后台管理员`核通过`后，总账户可以登陆商城

3.总账户可以创建`子账户`，创建后即可登陆使用，`子账户`也是手机号注册，不需要手机号验证码验证

4.总账户可以`增删改查`子账户信息，进行管理。

5.后台加入账户审核功能，以及查看子账户，总账户的列表，以及搜索过滤等。

二：总账户下单流程

1.总账户把产品加入购物车，创建订单，创建订单的时候，可以上传`zip文件包`


2.总账户可以直接进行`站内余额`支付

3.订单`发货`


三：子账户下单流程


1.子账户将产品加入购物车，创建订单，创建订单的时候，可以上传`zip文件包`

2.子账户创建订单完成后`不可以`进行支付，因此，创建订单后页面跳转到`账户中心`-`订单中心`，可以查看自己下的订单，
但是无法进行支付，需要等待总账户进行`审核`

3.总账户可以看到子账户创建的订单，进行`审核`

4.总账户`审核通过`后，子账户可以进行`支付操作`（子账户订单列表出现支付按钮），共享总账户的余额额度进行支付，当余额充足，即可支付成功

5.订单发货

6.总账户可以看到所有的子账户的订单，以及自己下的订单信息。

7.总账户支付，只能使用`站内余额`支付，`不能`使用微信支付宝等支付渠道

8.商城后台，可以看到所有的订单，可以根据`总账户`，`子账户`进行搜索，查看相应的订单信息

9.商城后台订单列表，可以下载用户创建订单上传的`zip文件包`，查看订单文件内容。

四：售后体系

1.售后退货，由`子账户`发起，不能由总账户发起

2.子账户发起后，售后`审核通过`后，用户可以进行退货商品发货操作

3.商家收货后，进行退货退款，退款的部分，将`站内余额`返还给`总账户`的`站内钱包`。

四：钱包部分

1.只有总账户可以进行`钱包充值`，子账户没有钱包部分

2.子账户可以查看总账户的钱包总额，子账户共享总账户的所有额度。

3.账户余额必须是正数，不允许`负数`订单扣款。

4.总账户可以查看`站内余额`的金额，`站内余额`变动历史等，子账户不可以查看`站内余额`变动历史

5.总账户可以线下打款，收到款后，管理员后台进行`站内余额`的手动充值，注意，不允许总账户线上直接充值

6.后台可以看到各个账户的`站内余额`变动列表。

五：订单流水导出

1.总账户可以导出订单信息以及订单产品信息，导出`excel表格`

2.总账户可以导出订单信息以及订单产品信息，导出`excel表格`

六：后台部分

1.后台可以直接更改首页`头部导航`

2.首页模版不需要 人气单品这些。













































