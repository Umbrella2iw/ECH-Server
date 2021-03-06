## 校疫小助手 服务端源码

### 简介

本项目是2020年微信小程序应用开发赛华东赛区二等奖作品`校疫小助手`的服务端。

`校疫小助手`小程序端开源准备中，将会在后续附上仓库链接。（预计今年年底开源）

开源版本是经过优化的，包括删除了冗余代码和敏感信息等，与比赛版本并非完全一致。

时间原因，开源版本只经过粗略的接口测试，并不保证所有接口都能够正常运作，如发现接口存在bug，欢迎提Issue以及Pull Request。

#### 技术栈

编程语言：JavaScript

使用框架：Express

ORM：Sequelize

#### 特点

##### 自动路由

本项目在服务初始化时，将会自动遍历routes文件夹下的所有路由配置文件，并挂载到Express实例中。在创建新路由时仅需让路由文件导出一个数组即可，从而达到减少app.js代码量的目的，同时也易于配置。

##### 完整注释

本项目所有的路由和控制器函数都有完整的JSDoc注释。

##### 自研表单验证工具

比赛版本的表单校验写法过于繁琐，故考虑自行编写一个表单校验类进行数据的校验。

未参考过express-validator，该校验工具类支持自定义校验规则，扩展性强。

### 如何部署

请看项目根目录下的[部署教程](./deployment.md)。

### 声明

项目开源仅供Node.js初学者学习，所有代码均不可用于个人项目和商业项目。

获奖作品仅开源服务器端和小程序端代码，作品相关文档和视频不公开。

作品代码版权属于参赛队伍MemoryLeak全体成员