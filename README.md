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
  <img src="http://wenhui012.images.nxptdn.com/充电平台/diagram/1.jpg"/>

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
### 后台
<table>
    <tr>
        <td><img src="http://wenhui012.images.nxptdn.com/%E5%85%85%E7%94%B5%E5%B9%B3%E5%8F%B0/pc/1%20%E9%A6%96%E9%A1%B5.png"/></td>
    </tr>
    <tr>
            <td><img src="http://wenhui012.images.nxptdn.com/%E5%85%85%E7%94%B5%E5%B9%B3%E5%8F%B0/pc/2%20%E7%94%A8%E6%88%B7%E7%BB%9F%E8%AE%A1.png"/></td>
        </tr>
    <tr>
        <td><img src="http://wenhui012.images.nxptdn.com/%E5%85%85%E7%94%B5%E5%B9%B3%E5%8F%B0/pc/2-1%20%E8%AE%BE%E5%A4%87%E7%AE%A1%E7%90%86%EF%BC%88%E7%BB%9F%E8%AE%A1%EF%BC%89.png"/></td>
    </tr>
    <tr>
        <td><img src="http://wenhui012.images.nxptdn.com/%E5%85%85%E7%94%B5%E5%B9%B3%E5%8F%B0/pc/2-3%20%E9%94%80%E5%94%AE%E7%BB%9F%E8%AE%A1.png"/></td>
    </tr>
    <tr>
        <td><img src="http://wenhui012.images.nxptdn.com/%E5%85%85%E7%94%B5%E5%B9%B3%E5%8F%B0/pc/2-2%20%E8%AE%BE%E5%A4%87%E7%AE%A1%E7%90%86%EF%BC%88%E5%9C%B0%E5%9D%80%EF%BC%89.png"/></td>
    </tr>
</table>

### 用户端
<table>
    <tr>
        <td><img src="http://wenhui012.images.nxptdn.com/%E5%85%85%E7%94%B5%E5%B9%B3%E5%8F%B0/mobile/0%20%E8%BE%93%E5%85%A5%E8%AE%BE%E5%A4%87%E7%A0%81.png"/></td>
        <td><img src="http://wenhui012.images.nxptdn.com/%E5%85%85%E7%94%B5%E5%B9%B3%E5%8F%B0/mobile/0%20%E9%A6%96%E9%A1%B5.png"/></td>
    </tr>
    <tr>
        <td><img src="http://wenhui012.images.nxptdn.com/%E5%85%85%E7%94%B5%E5%B9%B3%E5%8F%B0/mobile/1%20%E6%89%AB%E6%8F%8F.png"/></td>
        <td><img src="http://wenhui012.images.nxptdn.com/%E5%85%85%E7%94%B5%E5%B9%B3%E5%8F%B0/mobile/1%20%E7%BB%91%E5%AE%9A%E6%89%8B%E6%9C%BA%E5%8F%B7.png"/></td>
    </tr>
    <tr>
        <td><img src="http://wenhui012.images.nxptdn.com/%E5%85%85%E7%94%B5%E5%B9%B3%E5%8F%B0/mobile/2%20%E6%89%AB%E7%A0%81%E6%88%90%E5%8A%9F.png"/></td>
        <td><img src="http://wenhui012.images.nxptdn.com/%E5%85%85%E7%94%B5%E5%B9%B3%E5%8F%B0/mobile/%E6%8F%90%E7%8E%B0.png"/></td>
    </tr>
    <tr>
        <td><img src="http://wenhui012.images.nxptdn.com/%E5%85%85%E7%94%B5%E5%B9%B3%E5%8F%B0/mobile/3%20%E6%8C%89%E5%B0%8F%E6%97%B6%E6%94%B6%E8%B4%B9%E6%A0%87%E5%87%86.png"/></td>
        <td><img src="http://wenhui012.images.nxptdn.com/%E5%85%85%E7%94%B5%E5%B9%B3%E5%8F%B0/mobile/4%20%E6%94%AF%E4%BB%98%E6%88%90%E5%8A%9F%E5%A4%87%E4%BB%BD.png"/></td>
    </tr>
    <tr>
        <td><img src="http://wenhui012.images.nxptdn.com/%E5%85%85%E7%94%B5%E5%B9%B3%E5%8F%B0/mobile/5%20%E4%BD%99%E9%A2%9D%E5%85%85%E5%80%BC.png"/></td>
        <td><img src="http://wenhui012.images.nxptdn.com/%E5%85%85%E7%94%B5%E5%B9%B3%E5%8F%B0/mobile/6%20%E6%88%91%E7%9A%84%281%29.png"/></td>
    </tr>
</table>

### 代理商
<table>
    <tr>
        <td><img src="http://wenhui012.images.nxptdn.com/%E5%85%85%E7%94%B5%E5%B9%B3%E5%8F%B0/dailishang/1%20%E4%BB%A3%E7%90%86%E5%95%86%E7%99%BB%E5%BD%95.png"/></td>
        <td><img src="http://wenhui012.images.nxptdn.com/%E5%85%85%E7%94%B5%E5%B9%B3%E5%8F%B0/dailishang/2%20%E4%BB%A3%E7%90%86%E5%95%86%E5%8A%9F%E8%83%BD%E5%88%97%E8%A1%A8.png"/></td>
    </tr>
    <tr>
        <td><img src="http://wenhui012.images.nxptdn.com/%E5%85%85%E7%94%B5%E5%B9%B3%E5%8F%B0/dailishang/3-1%20%E8%AE%BE%E5%A4%87%E7%AE%A1%E7%90%86.png"/></td>
        <td><img src="http://wenhui012.images.nxptdn.com/%E5%85%85%E7%94%B5%E5%B9%B3%E5%8F%B0/dailishang/3-2%20%E8%AE%BE%E5%A4%87%E7%AE%A1%E7%90%86%EF%BC%88%E5%B1%95%E5%BC%80%EF%BC%89.png"/></td>
    </tr>
    
    
</table>


## 十一，如何部署
```
请参考每个工程都有READEME.md文档（详细部署文档）
```
## 十二，行者智能充电桩物联网云平台由宁夏普天动能信息技术有限公司投资建设。
## 十三，代码贡献者鸣谢
京东(JD) 资深java工程师  资深java工程师 郭亮波  芯正科技 CEO感谢的人很多
征得各位同意我们发布了V2.1版本，希望更多的跟个人和企业减少重复造轮子
减少投入。
