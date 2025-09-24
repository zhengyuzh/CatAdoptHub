# CatAdoptHub
流浪猫领养系统的设计与实现 【系统介绍 + 使用说明 】 <br>

## 系统介绍

### 一、系统功能规划  <br>
1. 用户端（小程序端） <br>
● 首页 : 公告轮播（如“今日新到流浪猫”“领养须知”）; 猫咪推荐（卡片式展示） <br>
● 猫咪管理 : 猫咪列表：支持分类（按年龄、健康状态）、搜索、分页; 猫咪详情：展示照片、简介、健康状况、是否已被认领 <br>
● 认领功能 : 认领申请：点击“认领”按钮提交申请; 认领记录查看：查看审核状态、通过/拒绝进度; 取消认领/完成认领 <br>
● AI功能 : 对话功能：可以咨询领养相关事情。（接入大模型对话功能） <br>
● 我的 : 我的资料、联系方式、地址 ; 我的认领记录、我的收藏 ；反馈与建议 <br>

2. 管理端（Web 后台 SpringBoot + Vue） <br>
● 猫咪分类管理（新增、编辑、删除、查询） <br>
● 猫咪信息管理（新增、编辑、删除、上传照片） <br>
● 认领申请管理（审核、通过、拒绝） <br>
● 公告管理、轮播图管理 <br>
● 反馈信息管理 <br>
● 用户管理 <br>

### 二、技术架构设计  <br>
1. 小程序端  <br>
● 框架：原生微信小程序    <br>
● UI：使用原生组件    <br>
● 接口：RESTful API（通过 wx.request 请求）  <br>

2. 后端  <br>
● 框架：Spring Boot + MyBatis-Plus  <br>
● 权限：JWT 登录验证  <br>
● 数据库：MySQL 5.7+  <br>
● 缓存：Redis（加速查询）  <br>
● 文件存储：OSS 或本地，支持图片上传  <br>

3. 管理后台
● Vue 2 + Element UI   <br>
● 登录权限：Token 校验  <br>
● 表格分页查询、数据管理、申请记录一应俱全   <br>

 ### 三、实现效果演示

实现效果演示: <a href ="https://www.bilibili.com/video/BV187JQzhErh/" >B站传送门</a>  <br>
后台管理实现效果演示: <a href ="https://mp.weixin.qq.com/s/tCoygQnXIfYXLC6U0C3_ww" >源码获取</a>  <br>
个人纯手搓，功能可以添加或者修改。可以添加本人联系方式：18348375641。<br>


# 实现效果部分截图
<img width="2560" height="1392" alt="image" src="https://github.com/user-attachments/assets/3dbb106a-2346-4253-8e99-b9b24c5fcfde" />

<img width="2560" height="1392" alt="image" src="https://github.com/user-attachments/assets/f07bc07c-302d-4243-814a-2f420a379a58" />

<img width="2560" height="1392" alt="image" src="https://github.com/user-attachments/assets/5ca0de90-92ac-42fb-b416-8925ffc5fc1c" />

<img width="2560" height="1392" alt="image" src="https://github.com/user-attachments/assets/5171bfb2-4ceb-4401-a650-ca3a8284091c" />

<img width="2560" height="1392" alt="image" src="https://github.com/user-attachments/assets/5003a7cd-0922-4c5b-b982-1fbaeee765ca" />

<img width="2560" height="1392" alt="image" src="https://github.com/user-attachments/assets/7c8744e9-1c1d-4e10-991c-e4ffb264519f" />

<img width="2560" height="1392" alt="image" src="https://github.com/user-attachments/assets/b4eb995d-0c53-4b9e-821d-8a1f33a7b7a9" />

<img width="2560" height="1392" alt="image" src="https://github.com/user-attachments/assets/96417ccb-6b66-47c2-90c9-584cf23f040c" />

<img width="2560" height="1392" alt="image" src="https://github.com/user-attachments/assets/b28e2aba-b387-409c-9a9e-5f00a63dfa81" />

<img width="2560" height="1392" alt="image" src="https://github.com/user-attachments/assets/9b0e6e3b-8a7d-4571-b97a-e3a7fbce7d30" />

<img width="2560" height="1271" alt="image" src="https://github.com/user-attachments/assets/f19a07f9-6ba6-4113-a771-1e9f61aaa484" />

<img width="2560" height="1271" alt="image" src="https://github.com/user-attachments/assets/7784ccbe-0100-4df8-a040-531056266a11" />

<img width="2560" height="1271" alt="image" src="https://github.com/user-attachments/assets/466f657d-454a-47da-8e8e-93f5c9fc544e" />







