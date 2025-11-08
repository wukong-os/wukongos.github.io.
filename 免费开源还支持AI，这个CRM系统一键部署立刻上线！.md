在众多企业管理软件中，CRM（客户关系管理系统）几乎是企业数字化转型的“中枢大脑”。但传统CRM系统价格高昂、部署复杂、维护困难，不仅让许多中小企业望而却步，也让不少团队陷入了“用不起、改不动、更新难”的尴尬境地。

而现在，一款免费开源、集成AI功能、支持一键部署的国产CRM系统——Wukong AI CRM，正在颠覆这一现状。

Wukong AI CRM 并不仅仅是“会部署”的系统，它还拥有完整的企业级功能：

1.	客户管理：统一存储客户资料、交互记录，轻松实现数据留存与共享；

2.	销售漏斗：可视化管理销售阶段，实时掌握业务进展；

3.	OA审批：内置多级审批流程，支持灵活配置；

4.	AI助手：自动分析客户行为、预测销售机会、生成智能报告；

5.	数据可视化：实时图表展示关键指标，助力管理决策。
 
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

对于追求高效率、低成本、可控安全的企业来说，这无疑是一款极具吸引力的解决方案。它让CRM不再是高门槛技术产品，而成为人人可用的数字化工具。

免费、开源、智能、一键上线——Wukong AI CRM 让企业管理更轻松，让AI赋能业务的未来从现在开始

🔗 引导开源地址

开源官网：www.wukongcrm.com

技术论坛：bbs.72crm.com

👉 悟空团队将持续以技术创新，赋能企业客户管理数字化升级。欢迎加入悟空开源社区，共建更智能的CRM生态！
