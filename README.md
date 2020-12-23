# EasyTestPlaform
1.服务请求：使用http工具类进行http请求。@feign注解调用微服务，调用配置文件中提供者的服务。
2.脚本分层：整个框架分为BaseTest-ServiceBaseTest-InterfaceTest，BaseTest影响整个工程的脚本，ServiceBaseTest可存放该服务公共方法/参数，公共前置操作及指定配置文件，InterfaceTest为用例实现类，通过继承让部分代码一次完成，多次使用。
3.失败重试：排除部分接口的网络传输影响。
4.数据驱动：通过@DataProvider对用例进行可重用多数据组合测试。
5.测试报告：Allure测试报告，直观显示成功/失败用例数，失败用例名，定位异常位置。
6.数据清理：jdbc访问数据库，还原或清除变动的数据。
7.钉钉推送：jenkins定时运行脚本，测试结果钉钉推送。
