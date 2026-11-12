# 基于SpringBoot+Vue的手办销售系统

![Spring Boot](https://img.shields.io/badge/-Spring%20Boot-6DB33F?style=flat-square&logo=spring-boot&logoColor=white) ![Vue3](https://img.shields.io/badge/-Vue3-grey?style=flat-square) ![MySQL](https://img.shields.io/badge/-MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white) ![MyBatis](https://img.shields.io/badge/-MyBatis-000000?style=flat-square&logo=mybatis&logoColor=white) 

## 项目介绍

本系统是一款面向二次元模玩爱好者与运营方的手办电商平台，针对通用商城难以覆盖的长周期定金预售、出荷延期通告、尾款补款履约、开箱买家秀与特典积分兑换等痛点，把现货直售、预售闭环、玩家社区、积分周边与后台经营分析整合到同一套前后端分离工程中，支撑从选购到发货售后的完整链路。

系统采用 SpringBoot + Vue 架构，区分普通玩家与系统管理员：玩家端完成浏览筛选、现货/定金下单、尾款补款、交流圈晒单、资讯阅读与积分兑换；管理员在经营大盘维护手办档案与分类厂商 IP、发货物流、售后审核、社区资讯与积分商城，并查看营收与热销趋势。适合作为毕设、课设与垂直电商数字化学习参考。

## 主要功能模块

- **用户认证与双角色分流**：玩家与管理员统一登录注册，JWT 鉴权；登录后按角色进入门户或经营后台，/admin 路由与接口双重隔离
- **门户首页大厅**：轮播 Banner、分类入口、热销与新品手办导流至商城与预售通知
- **全部手办检索**：按分类、厂商、IP 系列与关键词筛选，进入详情查看比例材质、现货价或预售定金
- **现货下单与余额支付**：加购购物车、结算支付；未支付可取消并回滚库存
- **定金预售与尾款补款**：预售商品先付定金，到货通告后补尾款，订单状态机贯穿履约
- **我的订单与售后**：查看现货/定金/尾款订单、确认收货；申请退款并上传凭证等待审核
- **玩家交流圈与买家秀**：发布展厅动态、点赞评论；商品评价沉淀口碑
- **资讯情报与积分俱乐部**：阅读模玩资讯；消费积分兑换周边并跟踪履约
- **收货地址与个人中心**：多地址维护、资料与余额相关能力集中管理
- **经营数据看板**：营收 KPI、销售趋势与热销榜，ECharts 辅助运营决策
- **商品与主数据中台**：手办上下架、分类/厂商/IP 系列维护、预售到货通告发布
- **订单发货与售后审核**：录入物流、审核退款；管理社区动态、资讯与积分商城兑换

## 技术架构

- **后端**：Spring Boot + MyBatis-Plus + JWT + Lombok + Hutool
- **前端**：Vue 3 + TypeScript + Vue Router + Pinia + Element Plus + Vite + ECharts
- **数据库**：MySQL

<!-- screenshots-start -->
## 系统截图

<img src="https://fanhua-yingcai.oss-cn-shanghai.aliyuncs.com/AutoUpload/screenshots/figureshop/%E7%99%BB%E5%BD%95%E9%A1%B5%E9%9D%A2.png" alt="登录页面" width="600" />

<img src="https://fanhua-yingcai.oss-cn-shanghai.aliyuncs.com/AutoUpload/screenshots/figureshop/%E7%94%A8%E6%88%B7%E9%A6%96%E9%A1%B5.png" alt="用户首页" width="600" />

<img src="https://fanhua-yingcai.oss-cn-shanghai.aliyuncs.com/AutoUpload/screenshots/figureshop/%E5%85%A8%E9%83%A8%E6%89%8B%E5%8A%9E.png" alt="全部手办" width="600" />

<img src="https://fanhua-yingcai.oss-cn-shanghai.aliyuncs.com/AutoUpload/screenshots/figureshop/%E6%89%8B%E5%8A%9E%E8%AF%A6%E6%83%85.png" alt="手办详情" width="600" />

<img src="https://fanhua-yingcai.oss-cn-shanghai.aliyuncs.com/AutoUpload/screenshots/figureshop/%E7%8E%A9%E5%AE%B6%E4%BA%A4%E6%B5%81%E5%9C%88.png" alt="玩家交流圈" width="600" />

<img src="https://fanhua-yingcai.oss-cn-shanghai.aliyuncs.com/AutoUpload/screenshots/figureshop/%E7%A7%AF%E5%88%86%E4%BF%B1%E4%B9%90%E9%83%A8.png" alt="积分俱乐部" width="600" />

<img src="https://fanhua-yingcai.oss-cn-shanghai.aliyuncs.com/AutoUpload/screenshots/figureshop/%E7%AE%A1%E7%90%86%E5%91%98%E4%BB%AA%E8%A1%A8%E7%9B%98.png" alt="管理员仪表盘" width="600" />

<img src="https://fanhua-yingcai.oss-cn-shanghai.aliyuncs.com/AutoUpload/screenshots/figureshop/%E6%89%8B%E5%8A%9E%E5%95%86%E5%93%81%E7%AE%A1%E7%90%86.png" alt="手办商品管理" width="600" />

<img src="https://fanhua-yingcai.oss-cn-shanghai.aliyuncs.com/AutoUpload/screenshots/figureshop/%E8%AE%BA%E6%96%87%E5%9B%BE1.png" alt="论文图1" width="600" />

<img src="https://fanhua-yingcai.oss-cn-shanghai.aliyuncs.com/AutoUpload/screenshots/figureshop/%E8%AE%BA%E6%96%87%E5%9B%BE2.png" alt="论文图2" width="600" />

<img src="https://fanhua-yingcai.oss-cn-shanghai.aliyuncs.com/AutoUpload/screenshots/figureshop/UML%E5%9B%BE%E5%88%97%E8%A1%A8.png" alt="UML图列表" width="600" />

<!-- screenshots-end -->

---

## 接毕业设计和论文

### 作者微信：vvsgxmn  (支持修改、 部署调试、 支持代做毕设)

### 接网站建设、小程序

### 选题+开题报告+任务书+程序定制+安装调试+论文+答辩ppt 都可以做

### 购买地址：[https://www.vvxx.love](https://www.vvxx.love)（vv毕设网）

### 支持 **一键生成 UML 图**：上传项目压缩包即可自动产出功能模块图、用例图、流程图、E-R 图、时序图等全套毕设图表。

### 提供 **免费配套软件下载 + 安装说明 + 部署教程**

![vv毕设网 - 一键画图](https://fanhua-yingcai.oss-cn-shanghai.aliyuncs.com/uml-draw.png)

<img src="https://fanhua-yingcai.oss-cn-shanghai.aliyuncs.com/image-20260825133349317.png" alt="image-20260825133349317" />

⚠️ Bug添加微信**免费修复**，免费修复。其他平台的私信一律不管（微信方便发送文件）
