FA-2.0数据收集
=================


> FA收集数据的介绍，包括收集数据的方式，以及收集数据的内容。


### FA收集数据的方式

1.收集数据的方式

FA的数据接收，分为2种，一种是`js`打点的方式接收，
另外一种就是商城服务端通过`Api`发送数据给`FA系统`，这样就可以使FA系统最大化的
接收用户的`行为记录`

1.1、`js打点`：fecshop已经将打点的代码写入，您只需要设置几行配置即可开启，
`js`收集有页面的数据，譬如：首页， 分类，产品，搜索，下单页面等等，
然后将数据传递给FA系统

1.2、商城服务端发送数据：对于没有页面的操作，但是又需要收集的数据，需要服务端
调用`api`发送数据，譬如：登录，注册，产品加入购物车，生成订单，
更改订单状态等

2.收集数据的内容

2.1、FA系统，会收集一些，类似于百度统计，`google analysis`的数据
，譬如：`浏览器`，`ip`，`设备`，`url`，`refer`等数据

2.2、`业务数据`，会收集用户的资料数据，行为数据等，譬如
产品页面会收集产品的`sku`，加入购物车操作会
收集`加入购物车的sku`，`个数`，以及`价格`，搜索页面会收集搜索的`关键词`以及
当前搜索页的产品总数，用户登录注册会收集用户的`email`信息，
用户下单会收集用户的`下单数据`

2.3、`营销广告数据`，广告员在做营销推广前，通过trace系统生成尾巴链接，
类似于：
http://fecshop.appfront.fancyecommerce.com/bags-accessories?fec_campaign=xxx&fec_content=94&fec_design=96&fec_medium=click&fec_source=EDM&fid=ac062761-5f43-46a7-9363-de1d53e1fc91
，广告发布后，用户通过该链接进入商城后，就会留下踪迹，
FA就会记录下来这些尾巴信息，用于广告数据计算

FA系统收集的数据非常全面，因此，根据业务类型，可以进行很多统计计算，
深入业务和业务紧密相连，
，这是 百度统计和google analysis无法做到的，


### 广告打点

广告员打的广告，一般都是需要花钱的，为了计算投资回报率，
广告员需要知道自己打的这个广告，是什么效果

广告员可以通过广告功能部分，将原始推广url复制进行，生成推广链接，譬如：
http://fecshop.appfront.fancyecommerce.com/bags-accessories?
fec_campaign=xxx&
fec_content=94&
fec_design=96&
fec_medium=click&
fec_source=EDM&
fid=ac062761-5f43-46a7-9363-de1d53e1fc91
，这个url的参数的意义如下：

`fid`：广告的唯一标示

`fec_source`：广告的渠道

`fec_medium`：广告的子渠道

`fec_campaign`：广告的活动名称

`fec_design`：广告中图片制作的美工的员工编号

`fec_content`：广告员的员工编号

当用户点击这个广告链接后，会在浏览器里面留下`cookie`，目前的设置，
该cookie会在用户的浏览器下面保存`15天`，15天内用户下的订单都属于该广告

这样就可以计算这个广告，每天的具体效果，然后`归并计算`，算出来
广告员每天的效果，广告渠道的的效果，等等、

该部分是为了方便广告员了解自己的广告的具体情况，找出来问题，
优化广告，找到好的广告渠道等等

另外也方便公司领导管理查看各个`广告员`的具体情况。






