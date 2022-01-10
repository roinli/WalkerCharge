## 场景演示 
https://haokan.baidu.com/v?pd=wisenatural&vid=13670646443722194884

## 代码贡献者鸣谢
京东(JD) 资深java工程师 杨膑 | 中科类脑 资深java工程师 郭亮波 | 芯正科技  CEO 梁亮 

## 源码地址  
https://gitee.com/dnxt111/walker.git
 

## 平台简介
行者（walker）是物联网快速开发平台，从（设备端-->服务端-->用户端）全链条场景，面向智能充电桩行业，毫无保留给个人及企业免费使用。
初衷，发现很多开源的产品缺东西，比如缺公众号，比如缺硬件对接的协议，我们希开源一套只要懂java的开发人员就能进行部署使用。

* 设备端采用netty
* 公众号界面采用Vue
* 公众号后端采用SpringBoot+Netty
* 运行后端采用SpringBoot、mybatis
* 运行后端系统前端采用 vue-admin-template
* db采用mysql


## 平台组成
* Netty服务：采用Netty采集硬件设备发送数据
* 公众号服务：操作微信公众号api
* 公众号UI界面:用户端操作界面
* 后台服务：管理端充电业务流程api
* 后台UI界面：管理端操作界面

## 组件关系列表
```
└─ walker                                                行者物联网快速开发平台
    ├─ open-smart-charge-operator-back                   后台服务
    ├─ open-smart-charge-operator-front                  后台UI界面
    ├─ open-smart-charge-wechat-font                     公众号UI界面
    └─ open-smart-charge-wechat-service                  三个部分（微信公众号服务 | Netty服务 | 业务服务)
        ├─ com.walker.netty                              Netty服务
        ├─ com.walker.web                                业务服务 
        ├─ com.walker.wx                                 微信公众号服务
```

## 内置功能

### 整体功能说明
用户使用微信公众号扫码设备进行设备充电或使用IC卡直接进行充电，充电结束进行扣款或充电时选择充电时长进行付费。
#### 运营端
1.  设备管理：
2.  规则管理：
3.  IC卡管理:
4.  代理商管理：
5.  ......陆续更新说明
#### 公众号
1.  微信扫码：扫码设备，选择充电端口，点击充电。
2.  微信充值：账号应最小50元金额，否则无法进行充电，以此保证用户进行快速充电。
3.  我的订单：我充值记录以及消费的订单
4.  ......陆续更新说明
#### 特别说明
目前产品已经落地实施，为了满足实际的应用场景，我们根据使用需求进行了大量的细节修改比如运营端进行设备退费，细节做了很多，满足实际场景需要。


## 在线体验

- admin/admin123456
- 陆陆续续收到一些打赏，为了更好的体验将尽快发布演示服务器。谢谢各位小伙伴。

演示地址：http://39.98.88.79:9762
## 演示图

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



## 如何部署
请参考每个工程都有READEME.md文档（详细的开发性文档，陆续更新）

## 行者充电桩快速开发平台交流群

* 微信：18601938676
* qq：544061884  

## 行者，物联网充电桩快速平台由芯正科技（宁夏）公司投资建设。
