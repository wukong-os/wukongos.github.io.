在数字化办公的时代，企业管理系统不仅要能用，还要能持续升级，适应业务发展和新需求。很多中小企业担心购买商业 CRM 后，系统难以升级或定制成本高昂。而 Wukong AI CRM 则提供了一个开源本地化解决方案，让企业在掌控数据安全的同时，也能持续升级系统功能。

如何选择适合的CRM

🌟 系统亮点

1.	一键部署：Docker 环境下快速启动，只需一条命令即可搭建完整系统。

2.	开源可控：源码完全开放，企业可自由部署、自由定制，数据100%掌握在自己手里。

3.	部署简单：仅需一条 Docker 命令，就能在笔记本或服务器上快速运行。

4.	数据驱动：内置 BI 报表、销售漏斗、趋势分析，让数据会“说话”。

5.	AI 加持：结合智能模型，可自动生成销售记录、客户分析报告。

6.	权限细分：支持组织架构、角色权限、流程审批等企业级管控。

7.	多端协作：支持网页端、移动端、企业微信打通，实现团队高效协同。

Wukong AI CRM 本地部署步骤

1. 准备环境

快速部署需要用到Docker，所以首先要安装Docker环境：

•	Windows 系统：

建议直接通过 Docker 官网 下载并安装 Docker Desktop。

该安装包已集成 Docker 和 Docker Compose，无需单独安装后者。

安装完成后，启动 Docker Desktop，即可同时启用 Docker 服务和 Docker Compose 功能。

 
•	Linux 系统：

可通过命令行脚本一键安装，执行以下命令：

bash <(curl -sSL https://linuxmirrors.cn/docker.sh)

此脚本会自动安装 Docker 引擎 和 Docker Compose，并配置必要的系统依赖（如容器网络、权限等）。

安装完成后，请手动启动 Docker 服务并设置开机自启：

systemctl start docker

systemctl enable docker

如安装失败，可前往官方论坛寻求帮助：https://bbs.72crm.com 

2. 开始安装Wukong AI-CRM 15

初始安装需求：悟空 CRM 安装要求电脑至少 4G 内存以上。

•	Windows 系统：

Windows 推荐使用 Wukong Core 应用 进行安装。

它支持可视化界面的一键部署，并可自动检测更新至最新版本。

首先在浏览器输入开源版本下载地址，http://www.wukongcrm.com/下载对应的应用
 
下载安装后，在桌面打开快捷方式即可看到界面
 
点击检查更新，等待更新完成，直到显示最新版本V15.0.1。
 
若为首次安装，更新完成后系统会自动在安装目录下载最新版本镜像并启动服务。

整个过程约需 10–20 分钟，请耐心等待。

请勿重复点击“检查更新”，否则会导致进度被重置。

•	Linux 系统：

Linux 系统安装需先确保已完成 Docker 与 Docker Compose 安装

第一步：从Github或者码云下载获取需要的镜像版本到服务器。完成 Docker 和 Docker Compose 安装后，通过以下命令启动项目：

cd Wukong_AI_CRM_15

第二步：进入 Docker 配置目录

cd docker

第三部：启动容器服务

docker compose up -d

命令解析：

docker compose：调用 Docker Compose 工具，用于管理多容器应用；

up：创建并启动 docker-compose.yml 中定义的所有服务；

-d：后台运行模式，容器在后台启动，不占用当前终端窗口。

若需查看实时日志，可使用以下命令：

docker compose logs -f
 

结语

一个能够持续升级的本地CRM，不仅让企业掌握核心数据、提高管理效率，还能随着业务发展不断优化功能，保持企业在市场竞争中的敏捷性。通过本地部署，企业可以实现安全、灵活、可持续的数字化管理，实现客户关系管理的最大化价值。
选择合适的本地CRM，就是选择一种长期可靠、可持续发展的企业数字化战略。
 
🔗 引导开源地址

开源官网：www.wukongcrm.com

技术论坛：bbs.72crm.com

👉 悟空团队将持续以技术创新，赋能企业客户管理数字化升级。欢迎加入悟空开源社区，共建更智能的CRM生态！
