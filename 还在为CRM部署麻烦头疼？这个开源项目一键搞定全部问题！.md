在企业管理中，CRM（客户关系管理系统）是核心工具，但很多商业 CRM 价格昂贵、定制化困难，部署复杂，让中小企业头疼。最近，我在 GitHub 上发现了一个国产开源的 Wukong AI CRM 系统，它不仅开源免费，还集成了 AI 智能，让销售和管理工作轻松高效。

核心特性一览

1.	灵活易用：表单、流程、权限可配置，实现销售自动化

2.	安全可控：支持私有化部署，企业数据完全掌控

3.	BI 加持：内置数据分析工具，低成本实现可视化报表

4.	AI 赋能：对接 MaxKB 智能体，支持 MCP 智能操作

5.	全链路管理：覆盖线索、客户、商机、产品全流程

6.	精细权限：支持组织架构、角色权限配置

7.	企业微信集成：打通企业微信，协作办公更顺畅

开源项目简介

Wukong AI CRM 的理念是帮助企业高效连接客户，实现精细化管理，而不仅仅是记录客户信息。

自主可控：数据存储在本地服务器或私有云，安全可靠

开源免费：不再依赖昂贵商业 CRM

AI 智能：通过 MaxKB 自动生成线索、智能录入跟进记录、智能查重

开源项目已在多家公司替代使用了多年商业 CRM，并完成了与 SQLBot、DataEase 的对接，未来将进一步开放更多智能功能。
 
如何使用 Wukong AI CRM

1. 准备环境

快速部署需要用到Docker，所以首先要安装Docker环境：

•	Windows 系统：

建议直接通过 Docker 官网 下载并安装 Docker Desktop。

网址为：https://www.docker.com

该安装包已集成 Docker 和 Docker Compose，无需单独安装后者。

安装完成后，启动 Docker Desktop，即可同时启用 Docker 服务和 Docker Compose 功能。
 
•	Linux 系统：

需通过命令行脚本一键安装，执行以下命令：

bash <(curl -sSL https://linuxmirrors.cn/docker.sh)

此脚本会自动安装 Docker 引擎和 Docker Compose，并配置必要的系统依赖（如容器网络、权限等）。

安装完成后，需手动启动 Docker 服务（通常命令为 systemctl start docker），并设置开机自启（systemctl enable docker）。

如果安装不成功，可以到官方论坛来提问解决：https://bbs.72crm.com 

2. 开始安装Wukong AI-CRM 15

初始安装需求：悟空 CRM 安装要求电脑至少 4G 内存以上。

•	Windows 系统：

Windows推荐使用Wukong Core 应用来安装，可视化图形界面一键安装部署，还可以支持实时更新最新版本。

首先在浏览器输入开源版本下载地址，http://www.wukongcrm.com/下载对应的应用
 
下载安装后，在桌面打开快捷方式即可看到界面
 
点击检查更新，等待更新完成，直到显示最新版本V15.0.1。
 
注意！！！如果是第一次安装，更新完成后将在安装文件夹下载对应的最新版本镜像，并启动服务，这个过程将会需要 10-20 分钟，请耐心等待，不要一直点击检查更新（否则将一直被重置）。

•	Linux 系统：

第一步：从Github或者码云下载获取需要的镜像版本到服务器。完成 Docker 和 Docker Compose 安装后，通过以下命令启动项目：

cd Wukong_AI_CRM_15

作用：切换到项目的根目录（假设项目文件夹名为 Wukong_AI_CRM_15，需根据实际下载的文件夹名称调整）


第二步：进入 Docker 配置目录

cd docker

作用：进入项目中存放 Docker 配置文件（如docker-compose.yml）的子目录。该目录包含启动容器所需的服务定义（如数据库、应用服务等）。

第三部：启动容器服务

docker compose up -d

命令解析：

docker compose：调用 Docker Compose 工具，用于管理多容器应用。

up：创建并启动 docker-compose.yml 中定义的所有服务容器（如 Web 应用、数据库、缓存等）。

-d（后台运行模式）：容器在后台启动，不占用当前终端窗口。若需查看实时日志，可去掉 -d，或后续使用 docker compose logs -f 命令。

结语

通过一台电脑、一键部署，我在一天内就完成了 CRM 系统上线任务，实现了老板的要求。对于中小企业来说，开源 CRM 系统不仅节省时间和成本，更能让企业快速迈入数字化管理时代。
 
🔗 引导开源地址

开源官网：www.wukongcrm.com

技术论坛：bbs.72crm.com

👉 悟空团队将持续以技术创新，赋能企业客户管理数字化升级。欢迎加入悟空开源社区，共建更智能的CRM生态！
