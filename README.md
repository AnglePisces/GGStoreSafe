# GGStoreSafe
VIPNCK.com--谷歌市场防下架方案、防抽检、防审核、防举报

它这个工具主要的核心点是帮助我们区分正常用户和抽检审核人员，接口接入非常简单，使用Http Get请求接入，正常用户接口返回0，抽检人员接口返回1。然后客户端只需要在启动后，先调用这个接口然后根据返回值判断是否是抽检人员：

1、返回值为0：那就是正常用户，直接给他显示正常的运营内容

2、返回值为1：就是抽检人员了，直接给他显示审核时候的正规内容
