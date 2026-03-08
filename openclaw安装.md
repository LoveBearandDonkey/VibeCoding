# OpenClaw 安装指南

## 安装openclaw

### Windows 系统搜索 cmd 打开命令行工具

#### 1. 安装依赖

自行安装(或让trae帮忙安装) node.js、Git

在命令行工具中，检查是否安装完成，可输入以下命令看下是否有版本号回复
```bash
node -v
```

```bash
git -v
```
上一步完成后，安装openclaw cli，需要等几分钟

```bash
npm install -g openclaw
```

#### 2. 开始安装openclaw

```bash
openclaw onboard
```
进入回合式安装，通过方向键和enter选择选项：  
1、I understand xxxx：选yes  
2、onboarding mode：选quickstart   
3、model provider：首先登录心仪的平台，确保能或有充值，或有赠送额度，就申请api key。不然申请api也无法用，后续安装完不好改供应商。比如这里选kimi.cn，控制台链接：https://platform.moonshot.cn/console/account
（选了后后续应该无法修改的所以要慎重）（问一下openclaw怎么安装技能用了2.2毛）    
4、选择kimi后，会提示输入api key，输入后回车即可。  
5、其他什么channel、skill等都选择skip   
6、search provide：选kimi  
7、最后安装完（可能会自动）打开打印内容中127那个网址  
8、【重要】：如果127这个提示打不开，是因为gateway无法自动运行，需要手动去电脑找到openclaw的安装目录，手动点开gateway命令脚本文件，刷新127网页即可  

#### 4. 其他
安装文档：https://docs.openclaw.ai/zh-CN/install  
卸载文档：https://docs.openclaw.ai/zh-CN/install/uninstall


## 安装技能
1、官方技能合集：https://clawhub.ai/  
2、目标技能：https://clawhub.ai/steipete/github  
3、手动下载安装包，解压到C:自己电脑目录\.openclaw\workspace\skills\github\  
4、问openclaw：我现在安装了哪些skill
