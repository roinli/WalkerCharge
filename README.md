# 行者智能充电桩物联网云平台
## 体验地址，star star ： [点我访问](https://gitee.com/dnxt111/walker.git)
## 开源最新版本要马上升级发布，先star在沟通，谢谢。


## 升级日志

## 一，场景演示 
https://haokan.baidu.com/v?pd=wisenatural&vid=13670646443722194884

## 二，源码地址  
https://gitee.com/dnxt111/walker.git
 
## 三，平台简介
行者物联云平台包括了公众号、H5、采集Server、后端平台，实现平台闭环，平台目前已经多次用于商业，完全采用Springboot、mysql、Netty、微信支付、微信退款等技术栈
* 行者智能充电桩物联网云平台，从（采集端-用户端-运营端）全业务场景，开源版本毫无保留给个人及企业免费使用。
* 初衷，发现很多开源的产品缺东西，比如缺公众号，比如缺硬件对接的协议，我们希开源一套只要懂java的开发人员就能进行部署使用。
* 初心：做了很多产品项目都商业落地了但是仅仅服务商业本身无法释放产品的价值，不在重复造轮子，让更多的企业和个人能够减少投入，先star欢迎讨论交流加群，微信18601938676
## 四，整体设计图（流程）
  <img src="http://shenqihezi.nxptdn.com/charge/diagram/1.jpg"/>

## 五，平台组成



----

```
* 采集端：使用Netty采集设备信息
* 用户端：使用小程序/H5作为载体
* 运营端：运行管理平台数据
```
## 六，软件架构
```
* 采集端：Netty、MQTT负责采集设备数据
* 用户端：①vue（前端） ②微信公众号API、SpringBoot、Mybatis(后端)
* 运行端：①vue-admin-template(前端) ②SpringBoot、Mybatis（后端）
* 数据库：MYSQL
```
## 七，代码结构
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

## 八，产品功能
```
### 整体功能说明
第一部分平台用户核心流程说明：
    用户使用微信公众号扫描设备，选择端口，
    选择充电时长微信支付费用或选择设备充电完成自动扣款两种模式，
    插上充电口充电。
第二部分代理商saas模式说明（可选）：
    平台开发代理商模式即代理商自行购买设备，代理商自行设置收费模式、自行计费、以及设备的管理等功能。

## 特别说明
目前产品已经落地实施，为了满足实际的应用场景，我们根据使用需求进行了大量的细节修改比如运营端进行设备退费，细节做了很多，满足实际场景需要。
```
## 九，团队计划
```
- 用心做产品，不以赚钱为目的。
- 搭建基础性行者物联网快速开发平台。
- 软件架构升级SpringCloud/产品细节优化
- 推广促进更多厂家和硬件开发者接入行者智能充电桩物联网云平台
- 以前做过：智能充电桩云平台，AI计算中心，智慧农业，智慧工业，高效节水，水肥一体化，污水处理，计量计费，水质检测，智慧大棚，农业项目
```
## 十，部分截图

<table>
    <tr>
        <td><img src="http://shenqihezi.nxptdn.com/charge/pc/1登录.png"/></td>
    </tr>
    <tr>
        <td><img src="http://shenqihezi.nxptdn.com/charge/pc/2统计.png"/></td>
    </tr>
     <tr>
        <td><img src="http://shenqihezi.nxptdn.com/charge/pc/3设备管理.png"/></td>
    </tr>
    <tr>
        <td><img src="http://shenqihezi.nxptdn.com/charge/mobile/卡管理2.png"/></td>
    </tr>
    <tr>
        <td><img src="http://shenqihezi.nxptdn.com/charge/mobile/扫码成功.png"/></td>
    </tr>
    <tr>
         <td><img src="http://shenqihezi.nxptdn.com/charge/mobile/提现.png"/></td>
    </tr>
    <tr>
        <td><img src="http://shenqihezi.nxptdn.com/wisdom/case/银川小区.jpg"/></td>
    </tr>
</table>


## 十一，如何部署
```
请参考每个工程都有READEME.md文档（详细部署文档）
```
## 十二，行者智能充电桩物联网云平台由宁夏普天动能信息技术有限公司投资建设。
## 十三，代码贡献者鸣谢
京东(JD) 资深java工程师  中科类脑 郭亮波  芯正科技 CEO感谢的人很多
征得各位同意我们发布了V2.1版本，希望更多的跟个人和企业减少重复造轮子
减少投入。
