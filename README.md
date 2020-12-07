 <p align="center">
      <img src="https://img.shields.io/badge/Release-V2.7.2-green.svg" alt="Downloads">
      <img src="https://img.shields.io/badge/JDK-1.8+-green.svg" alt="Build Status">
  <img src="https://img.shields.io/badge/license-Apache%202-blue.svg" alt="Build Status">
   <img src="https://img.shields.io/badge/Spring%20Cloud-Hoxton.SR7-blue.svg" alt="Coverage Status">
   <img src="https://img.shields.io/badge/Spring%20Boot-2.2.9.RELEASE-blue.svg" alt="Downloads">
   <a target="_blank" href="https://awcpx.vip">
   <img src="https://img.shields.io/badge/Author-Small%20Chill-ff69b4.svg" alt="Downloads">
 </a>
 <a target="_blank" href="https://awcpx.vip">
   <img src="https://img.shields.io/badge/Copyright%20-@awcpX-%23ff3f59.svg" alt="Downloads">
 </a>
 </p>  

## Springawcp微服务开发平台
* 采用前后端分离的模式，前端开源两个框架：[RUI](https://awcp.com/smallc/RUI) (基于 React、Ant Design)、[AUI](https://awcp.com/smallc/AUI) (基于 Vue、Element-UI)
* 后端采用SpringCloud全家桶，并同时对其基础组件做了高度的封装，单独开源出一个框架：[AWCPTool](https://awcp.com/chillzhuang/awcp-tool)
* [AWCPTool](https://awcp.com/chillzhuang/awcp-tool)已推送至Maven中央库，直接引入即可，减少了工程的臃肿，也可更注重于业务开发
* 集成Sentinel从流量控制、熔断降级、系统负载等多个维度保护服务的稳定性。
* 注册中心、配置中心选型Nacos，为工程瘦身的同时加强各模块之间的联动。
* 使用Traefik进行反向代理，监听后台变化自动化应用新的配置文件。
* 极简封装了多租户底层，用更少的代码换来拓展性更强的SaaS多租户系统。
* 借鉴OAuth2，实现了多终端认证系统，可控制子系统的token权限互相隔离。
* 借鉴Security，封装了Secure模块，采用JWT做Token认证，可拓展集成Redis等细颗粒度控制方案。
* 稳定生产了一年，经历了从Camden -> Greenwich的技术架构，也经历了从fat jar -> docker -> k8s + jenkins的部署架构
* 项目分包明确，规范微服务的开发模式，使包与包之间的分工清晰。

## 工程结构
``` 
AWCP
├── awcp-auth -- 授权服务提供
├── awcp-common -- 常用工具封装包
├── awcp-gateway -- Spring Cloud 网关
├── awcp-ops -- 运维中心
├    ├── awcp-admin -- spring-cloud后台管理
├    ├── awcp-develop -- 代码生成
├    ├── awcp-resource -- 资源管理
├    ├── awcp-seata-order -- seata分布式事务demo
├    ├── awcp-seata-storage -- seata分布式事务demo
├── awcp-service -- 业务模块
├    ├── awcp-desk -- 工作台模块 
├    ├── awcp-log -- 日志模块 
├    ├── awcp-system -- 系统模块 
├    └── awcp-user -- 用户模块 
├── awcp-service-api -- 业务模块api封装
├    ├── awcp-desk-api -- 工作台api 
├    ├── awcp-dict-api -- 字典api 
├    ├── awcp-system-api -- 系统api 
└──  └── awcp-user-api -- 用户api 
```

## 官网
* 官网地址：[https://awcpx.vip](https://awcpx.vip)
* 问答社区：[https://sns.awcpx.vip](https://sns.awcpx.vip)
* 会员计划：[Springawcp会员计划](https://gitee.com/smallc/Springawcp/wikis/Springawcp会员计划)
* 交流一群：`477853168`(满)
* 交流二群：`751253339`(满)
* 交流三群：`784729540`(满)
* 交流四群：`1034621754`(满)
* 交流五群：`946350912`

## 在线演示
* AUI-基于Vue：[https://AUI.awcpx.vip](https://AUI.awcpx.vip)
* RUI-基于React：[https://RUI.awcpx.vip](https://RUI.awcpx.vip)
* Archer-全能代码生成系统：[https://archer.awcpx.vip](https://archer.awcpx.vip)
* Caster-数据大屏展示系统：[https://data.avuejs.com](https://data.avuejs.com)

## 技术文档
* [Springawcp开发手册一览](https://gitee.com/smallc/Springawcp/wikis/Springawcp开发手册)
* [常见问题集锦](https://sns.awcpx.vip/article-14966.html)

## 项目地址
* 后端Gitee地址：[https://gitee.com/smallc/Springawcp](https://gitee.com/smallc/Springawcp)
* 后端Github地址：[https://github.com/chillzhuang/Springawcp](https://github.com/chillzhuang/Springawcp)
* 后端SpringBoot版：[https://gitee.com/smallc/Springawcp/tree/2.0-boot/](https://gitee.com/smallc/Springawcp/tree/2.0-boot/)
* 前端框架RUI(基于React)：[https://gitee.com/smallc/RUI](https://gitee.com/smallc/RUI)
* 前端框架AUI(基于Vue)：[https://gitee.com/smallc/AUI](https://gitee.com/smallc/AUI)
* 核心框架项目地址：[https://github.com/chillzhuang/awcp-tool](https://github.com/chillzhuang/awcp-tool)

## 用户权益
* 允许免费用于学习、毕设、公司项目、私活等。
* 代码文件需保留相关license信息。
* 禁止直接将本项目挂淘宝等商业平台出售。
* 非界面代码50%以上相似度的二次开源，二次开源需先联系作者。

## 如何启动
```
$ git clone https://gitee.com/smallc/AUI.git
$ cd AUI
# 安装
$ yarn install
# 启动
$ yarn run serve     
```

# 界面

## [awcpX](https://awcpx.vip/#/vip) 工作流一览
<table>
    <tr>
        <td><img src="https://gitee.com/smallc/Springawcp/raw/master/pic/awcpx-flow1.png"/></td>
        <td><img src="https://gitee.com/smallc/Springawcp/raw/master/pic/awcpx-flow2.png"/></td>
    </tr>
    <tr>
        <td><img src="https://gitee.com/smallc/Springawcp/raw/master/pic/awcpx-flow3.png"/></td>
        <td><img src="https://gitee.com/smallc/Springawcp/raw/master/pic/awcpx-flow4.png"/></td>
    </tr>
    <tr>
        <td><img src="https://gitee.com/smallc/Springawcp/raw/master/pic/awcpx-flow5.png"/></td>
        <td><img src="https://gitee.com/smallc/Springawcp/raw/master/pic/awcpx-flow6.png"/></td>
    </tr>
</table>

## [RUI](https://gitee.com/smallc/RUI) 界面一览
<table>
    <tr>
        <td><img src="https://gitee.com/smallc/Springawcp/raw/master/pic/RUI-main.png"/></td>
        <td><img src="https://gitee.com/smallc/Springawcp/raw/master/pic/RUI-menu.png"/></td>
    </tr>
    <tr>
        <td><img src="https://gitee.com/smallc/Springawcp/raw/master/pic/RUI-menu-edit.png"/></td>
        <td><img src="https://gitee.com/smallc/Springawcp/raw/master/pic/RUI-menu-icon.png"/></td>
    </tr>
    <tr>
        <td><img src="https://gitee.com/smallc/Springawcp/raw/master/pic/RUI-role.png"/></td>
        <td><img src="https://gitee.com/smallc/Springawcp/raw/master/pic/RUI-user.png"/></td>
    </tr>
    <tr>
        <td><img src="https://gitee.com/smallc/Springawcp/raw/master/pic/RUI-dict.png "/></td>
        <td><img src="https://gitee.com/smallc/Springawcp/raw/master/pic/RUI-log.png"/></td>
    </tr>
    <tr>
        <td><img src="https://gitee.com/smallc/Springawcp/raw/master/pic/RUI-locale-cn.png"/></td>
        <td><img src="https://gitee.com/smallc/Springawcp/raw/master/pic/RUI-locale-us.png"/></td>
    </tr>
</table>

## [AUI](https://gitee.com/smallc/AUI) 界面一览
<table>
    <tr>
        <td><img src="https://gitee.com/smallc/Springawcp/raw/master/pic/AUI-user.png"/></td>
        <td><img src="https://gitee.com/smallc/Springawcp/raw/master/pic/AUI-role.png"/></td>
    </tr>
    <tr>
        <td><img src="https://gitee.com/smallc/Springawcp/raw/master/pic/AUI-dict.png"/></td>
        <td><img src="https://gitee.com/smallc/Springawcp/raw/master/pic/AUI-dict-select.png"/></td>
    </tr>
    <tr>
        <td><img src="https://gitee.com/smallc/Springawcp/raw/master/pic/AUI-log.png"/></td>
        <td><img src="https://gitee.com/smallc/Springawcp/raw/master/pic/AUI-code.png"/></td>
    </tr>
</table>

## 监控界面一览
<table>
    <tr>
        <td><img src="https://gitee.com/smallc/Springawcp/raw/master/pic/springawcp-k8s1.png"/></td>
        <td><img src="https://gitee.com/smallc/Springawcp/raw/master/pic/springawcp-k8s2.png"/></td>
    </tr>
    <tr>
        <td><img src="https://gitee.com/smallc/Springawcp/raw/master/pic/springawcp-grafana.png"/></td>
        <td><img src="https://gitee.com/smallc/Springawcp/raw/master/pic/springawcp-harbor.png"/></td>
    </tr>
    <tr>
        <td><img src="https://gitee.com/smallc/Springawcp/raw/master/pic/springawcp-traefik.png"/></td>
        <td><img src="https://gitee.com/smallc/Springawcp/raw/master/pic/springawcp-traefik-health.png"/></td>
    </tr>
    <tr>
        <td><img src="https://gitee.com/smallc/Springawcp/raw/master/pic/springawcp-nacos.png"/></td>
        <td><img src="https://gitee.com/smallc/Springawcp/raw/master/pic/springawcp-sentinel.png"/></td>
    </tr>
    <tr>
        <td><img src="https://gitee.com/smallc/Springawcp/raw/master/pic/springawcp-admin1.png"/></td>
        <td><img src="https://gitee.com/smallc/Springawcp/raw/master/pic/springawcp-admin2.png"/></td>
    </tr>
    <tr>
        <td><img src="https://gitee.com/smallc/Springawcp/raw/master/pic/springawcp-swagger1.png"/></td>
        <td><img src="https://gitee.com/smallc/Springawcp/raw/master/pic/springawcp-swagger2.png"/></td>
    </tr>
</table>

## 关注我们
![](https://images.gitee.com/uploads/images/2019/0330/065148_f0ada806_410595.jpeg)
