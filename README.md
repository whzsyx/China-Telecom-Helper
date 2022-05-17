# China-Telecom-Helper 中国电信助手
中国电信助手

每日签到(随机金豆),每日登录奖励领取(5金豆),查看我的云盘(10金豆),翻牌 (10金豆),查看我的订单 (5金豆),打开消息 (100金豆),当日分享 (50金豆),浏览生活频道 (5金豆),查看我的金豆 (5金豆),关注直播 (5金豆),观看直播15s (5金豆),打开消息 (100金豆),答问卷 (100金豆),部分任务需要手动操作完成


![image.png](https://pic.rmb.bdstatic.com/bjh/7367f58ef56656fac3c1ed462e658bb9.png)


免费使用,禁止买卖,仅限用于学习和研究目的；不得用于商业或者非法用途，否则，一切后果请用户自负。您必须在下载后的24个小时之内，从您的电脑中彻底删除上述内容。

## 前言


活动规则请自行至电信官方查看,不作解释.

金豆自动兑换话费模块可能涉及盈利,已移除.可自行手动兑换,每月固定15元,其他不定时活动0~200.



## 配置运行

程序同目录下创建 config.json 文件 (Linux 需要同时 chmod +x China-Telecom-Helper_0.1_linux_amd64)

phone,cookie,para自行抓包获取

systime默认即可,也可更换国内cdn,

```
cloudflare 全球cdn加速  

https://cloudflare.api.isoyu.com/time/SysTime/?appCode=B586A14C4EC466D33682F8626CCB3794&auturl=api.isoyu.com&num=13

国内 cdn加速

https://api.isoyu.com/time/SysTime/?appCode=B586A14C4EC466D33682F8626CCB3794&auturl=api.isoyu.com&num=13
```

### 完整示例

```
{
  "users": [
    {
      "cookie": "cookie",
      "para": "para",
      "phone": 13800138000,
      "systime": "https://cloudflare.api.isoyu.com/time/SysTime/?appCode=B586A14C4EC466D33682F8626CCB3794&auturl=api.isoyu.com&num=13",
      "github": "https://github.com/insoxin/China-Telecom-Helper"

    }
  ]
}
```
### 试运行

Linux 
```
wget https://github.com/insoxin/China-Telecom-Helper/releases/download/0.1/China-Telecom-Helper_0.1_linux_amd64
wget https://github.com/insoxin/China-Telecom-Helper/releases/download/0.1/config.json
chmod +x China-Telecom-Helper_0.1_linux_amd64
./China-Telecom-Helper_0.1_linux_amd64
```
config.json需要填写所有参数

### 定时执行
Linux 可使用 Crontab 设置定时任务

windows可使用 系统任务计划程序 设置定时任务


## 运行截图


![image.png](https://pic.rmb.bdstatic.com/bjh/7367f58ef56656fac3c1ed462e658bb9.png)

```
中国电信助手v0.1

免费使用,禁止买卖,仅限用于学习和研究目的；不得用于商业或者非法用途，否则，一切后果请用户自负。您必须在下载后的24个小时之内，从您的电脑中彻底删除上述内容。

下载更新:https://github.com/insoxin/China-Telecom-Helper

正在查找配置文件

配置已找到,正在解析


Phone: 13800138000
Cookie: cookie
Para: para


开始获取远程时间:
2022-05-17 15:54:58
1652774098787


开始800金豆兑换5元话费:未找到参数设置,自动跳过
开始400金豆兑换2元话费:未找到参数设置,自动跳过
开始200金豆兑换1元话费:未找到参数设置,自动跳过

开始第1次喂食:今天已达到最大喂食次数
开始第2次喂食:今天已达到最大喂食次数
开始第3次喂食:今天已达到最大喂食次数
开始第4次喂食:今天已达到最大喂食次数
开始第5次喂食:今天已达到最大喂食次数
开始第6次喂食:今天已达到最大喂食次数
开始第7次喂食:今天已达到最大喂食次数
开始第8次喂食:今天已达到最大喂食次数
开始第9次喂食:今天已达到最大喂食次数
开始第10次喂食:今天已达到最大喂食次数


每日签到:操作成功
每日登录奖励领取(5金豆):操作成功
查看我的云盘(10金豆):操作成功
翻牌 (10金豆):操作成功
查看我的订单 (5金豆):操作成功
打开消息 (100金豆):操作成功
当日分享 (50金豆):操作成功
浏览生活频道 (5金豆):操作成功
查看我的金豆 (5金豆):操作成功
关注直播 (5金豆):操作成功
取消关注直播:操作成功
观看直播15s (5金豆):打开中国电信直播
观看15s结束
打开消息 (100金豆):操作成功
答问卷 (100金豆):操作成功

所有已完成任务领取金豆成功,部分任务需要手动操作完成,具体请看GitHub文档.程序将在清理后台进程后关闭.

```