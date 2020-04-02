---
description: 使用此项目前需要修改SSP面板的地方
---

# 面板的修改

## 源代码：

* [SSPanel-Uim](https://github.com/Anankke/SSPanel-Uim): [https://github.com/du5/SSPanel-Uim-Trojan/commit/c2c88302](https://github.com/du5/SSPanel-Uim-Trojan/commit/c2c88302) （支持WEBAPI对接
* [Malio](https://gitlab.com/masivro/malio-theme-for-sspanel): [https://gitlab.com/Gtary/malio-theme-for-sspanel/-/commit/22168a26](https://gitlab.com/Gtary/malio-theme-for-sspanel/-/commit/22168a26) （WEBAPI对接正在适配

{% hint style="warning" %}
修改内容请自行比对，远程协助比对安装请额外支付 30 USDT
{% endhint %}

## 节点编辑

Server 格式: google.com;port=1443\|host=baidu.com

> google.com 改为你的真是机器解析IP或域名
>
> port 改为你后端开启的端口
>
> baidu.com 改为你的 trojan 服务器证书 peer/sni 证书名

## 计划任务

> 仅 MYSQL 对接时需要

```bash
*/1 * * * * php xcat checkjob > /dev/null
*/1 * * * * php xcat trojan_checkjob > /dev/null
```

