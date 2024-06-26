
# 基于图像识别的自动化测试框架
设计并实现一个基于UI自动化、接口自动化、PO模式、数据驱动、关键字驱动、持续集成与持续发布、图像识别等技术的自动化测试框架。本框架选用 Selenium+Requests+pytest框架作为控制层进行逻辑验证，YAML作为持久层进行测试数据的存储，利用Logging 埋点记录日志，基于 Git+Jenkins 实现持续集成，之后在显示层通过钉钉机器人将漂亮的Allure测试报告持续交付至钉钉群，最终实现了自动化测试。


![](https://img.shields.io/badge/python-%3E%3D3.9-brightgreen)
![](https://img.shields.io/badge/License-MIT-blue)
![](https://img.shields.io/badge/version-4.0-yellowgreen)

推荐书籍1：[Selenium自动化测试完全指南：基于Python_赵卓](https://weread.qq.com/web/bookDetail/d5c32d2072462defd5c7805)

推荐书籍2：[饿了么质量体系搭建实战_张丙振、檀飞翔](https://weread.qq.com/web/bookDetail/9cb32f10721a48be9cbdc2a)

# 自动化测试框架设计与优化思路
![image](img/框架设计与优化思路.jpg)
---
# 项目基本情况
[V1.0版本](https://github.com/huangyong2002/Hy-UiTest-Framework/tree/V1.0)  
- [x] 基于PO设计模式构建项目
- [x] 增加浏览器驱动的封装
- [x] 基于WebDriverManager实现浏览器驱动的自动下载

[V2.0版本](https://github.com/huangyong2002/Hy-UiTest-Framework/tree/V2.0)  
- [x] 使用yaml配置文件来实现测试数据的统一管理
- [x] 实现对selenium常用操作的二次封装（获取元素、等待页面完全加载完成、等待页面元素消失和出现、跳转地址、元素是否出现、元素填值、元素点击）

[V3.0版本](https://github.com/huangyong2002/Hy-UiTest-Framework/tree/V3.0)  
- [x] 基于fixture和conftest实现用例层浏览器的初始化设置和结束设置
- [x] 参数化部分测试用例
- [x] 基于Opencv实现图像识别
- [x] 基于Allure生成测试报告
- [x] 基于Jenkins实现定时执行和持续集成

[V4.0版本](https://github.com/huangyong2002/Hy-UiTest-Framework/tree/V4.0)
- [x] 支持失败截图及重试机制
- [x] 增加日志处理机制
- [x] 支持处理图形验证码
- [x] 支持分布式执行测试用例并将测试报告自动发送至钉钉群
- [x] 支持MySQL数据库校验
- [ ] 基于Redis存储测试结果（测试用例名、测试结果、自动化测试进度等）并发送至钉钉群


# 目录介绍
> base: 包括selenium二次封装以及各个页面元素的封装
> 
> common: 包括部分通用方法
> 
> config: 包括driver方法和配置文件
> 
> img: 存放图片
> 
> logs: 日志相关
> 
> page: 页面类
> 
> testcase: 测试用例

# 项目演示
https://www.bilibili.com/video/BV1Gv4y1e77V?share_source=copy_web

