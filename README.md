# 行者智能充电桩物联网云平台
## 体验地址，star star ： [点我访问](https://gitee.com/dnxt111/walker.git)

## 一，场景演示 
https://haokan.baidu.com/v?pd=wisenatural&vid=13670646443722194884

## 二，源码地址  
https://gitee.com/dnxt111/walker.git
 
## 三，平台简介
行者智能充电桩物联网云平台，从（采集端-用户端-运营端）全业务场景，开源版本毫无保留给个人及企业免费使用。
初衷，发现很多开源的产品缺东西，比如缺公众号，比如缺硬件对接的协议，我们希开源一套只要懂java的开发人员就能进行部署使用。

## 四，平台组成
```
* 采集端：使用Netty采集设备信息
* 用户端：使用小程序/H5作为载体
* 运营端：运行管理平台数据
```
## 五，软件架构
```
* 采集端：Netty、MQTT负责采集设备数据
* 用户端：①vue（前端） ②微信公众号API、SpringBoot、Mybatis(后端)
* 运行端：①vue-admin-template(前端) ②SpringBoot、Mybatis（后端）
* 数据库：MYSQL
```
## 六，目录组成
```
└─ walker                                                行者智能充电桩物联网云平台
    ├─ open-smart-charge-operator-back                   运营端：接口
    ├─ open-smart-charge-operator-front                  运营端：前端
    ├─ open-smart-charge-wechat-font                     用户端：前端
    └─ open-smart-charge-wechat-service                  ①采集端：Netty ②用户端：后端 ③用户端：微信API 
        ├─ com.walker.netty                              ①采集端：Netty
        ├─ com.walker.web                                ②用户端：后端
        ├─ com.walker.wx                                 ③用户端：微信API
```

## 七，内置功能
```
### 整体功能说明
第一部分平台用户核心流程说明：
    用户使用微信公众号扫描设备，选择端口，选择充电时长微信支付费用或选择设备充电完成自动扣款两种模式，插上充电口充电。
第二部分代理商saas模式说明（可选）：
    平台开发代理商模式即代理商自行购买设备，代理商自行设置收费模式、自行计费、以及设备的管理等功能。

## 特别说明
目前产品已经落地实施，为了满足实际的应用场景，我们根据使用需求进行了大量的细节修改比如运营端进行设备退费，细节做了很多，满足实际场景需要。
```
## 八，团队计划
```
- 用心做产品，不以赚钱为目的。
- 搭建基础性行者物联网快速开发平台。
- 软件架构升级SpringCloud/产品细节优化
- 推广促进更多厂家和硬件开发者接入行者智能充电桩物联网云平台
- 以前做过：智能充电桩云平台，AI计算中心，智慧农业，智慧工业，高效节水，水肥一体化，污水处理，计量计费，水质检测，智慧大棚，农业项目
```
## 九，部分系统图

<table>
    <tr>
        <td><img src="http://shenqihezi.nxptdn.com/1登录.png"/></td>
        <td><img src="http://shenqihezi.nxptdn.com/2统计.png"/></td>
        <td><img src="http://shenqihezi.nxptdn.com/3设备管理.png"/></td>
    </tr>
    <tr>
        <td><img src="http://shenqihezi.nxptdn.com/卡管理2.png"/></td>
        <td><img src="http://shenqihezi.nxptdn.com/扫码成功.png"/></td>
        <td><img src="http://shenqihezi.nxptdn.com/提现.png"/></td>
    </tr>
</table>


## 十，如何部署
```
请参考每个工程都有READEME.md文档（详细的开发性文档）
```
## 十一，行者智能充电桩物联网云平台交流群
```
* 微信：18601938676
* qq：544061884  
```
## 十二，行者智能充电桩物联网云平台由芯正科技（宁夏）公司投资建设。

## 十三，代码贡献者鸣谢
京东(JD) 资深java工程师  中科类脑 郭亮波  芯正科技 CEO
