# 网站状态页失效

最近没时间看小站，今天登录发现小站的监控页面出错了，到底是发生了什么让监控页面出错了呢？

后来在收件箱发现了一封来自 UptimeRobot 的未读邮件，**状态页面自定义域名需要升级到收费版本**。

&gt; The main reason is the huge load on our systems and the issuance and renewal of SSL certificates hitting several 3rd party service rate limits while slowing down the process of activating new Status pages significantly.
&gt; We still want to offer a lot of useful free services to our community and users, but we need to focus on quality and reliability too.

如果不升级到 PRO，**免费计划中状态页面链接的自定义域的支持将于 2021 年 5 月  5 日停止服务，只能使用默认链接（例如stats.uptimerobot.com/xxx），之前链接的域将指向 “404 错误” 页面**。

&gt; What does it mean for you?
&gt;
&gt; After May 5th, 2021 linked domains will point to the “error 404” page.No worries though. Here’s what you can do:
&gt;
&gt; - Switch to use free status page under UptimeRobot’s domain(e.g. stats.uptimerobot.com/statusPageID)- don’t forget to change the links on your website.
&gt; - Continue using the linked domain by upgrading to a PRO plan. With the PRO plan you will also get Status page customizations, unlimited number of Status pages, 1-minute monitor intervals, SSL monitoring &amp; alerting and much more.


---

> 作者:   
> URL: https://blog.wenyi.org/posts/status-page-invalidated/  

