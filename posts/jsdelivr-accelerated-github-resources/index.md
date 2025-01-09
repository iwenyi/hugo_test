# JsDelivr 加速 Github 资源

## 介绍

CDN 的全称是 Content Delivery Network，即[内容分发网络](https://baike.baidu.com/item/%E5%86%85%E5%AE%B9%E5%88%86%E5%8F%91%E7%BD%91%E7%BB%9C/4034265)。CDN 是构建在现有网络基础之上的智能虚拟网络，依靠部署在各地的边缘服务器，通过中心平台的负载均衡、内容分发、调度等功能模块，使用户就近获取所需内容，降低网络拥塞，提高用户访问响应速度和命中率。CDN 的关键技术主要有内容存储和分发技术。[（百度百科）](https://baike.baidu.com/item/CDN)

因为某些原因，Github 在国内访问不稳定，下载仓库资源非常缓慢，可以用 CDN 解决这个问题。

jsDelivr 是免费的 CDN，而且最重要的是在中国大陆唯一有许可证的公共 CDN，速度非常快。

![jsDelivr 官网](1.webp)

## 使用

**引用 jsDelivr:**

    https://cdn.jsdelivr.net/gh/user/repo@version/file

详细规则访问官网：
https://www.jsdelivr.com

### 图床

例如：

`https://cdn.jsdelivr.net/gh/iwenyi/tuchuang/UptimeRobot%E9%A1%B5%E9%9D%A2404%E5%A4%B4%E5%9B%BE.png#vwid=1394&amp;vhei=751`

效果：

![头图 404](2.webp)

这样可以使用 Github&#43;jsDelivr 搭建图床，我之前写过：[https://blog.wenyi.org/posts/website-log-three/](https://blog.wenyi.org/posts/website-log-three/)

### 下载

例如：`https://cdn.jsdelivr.net/gh/iwenyi/bing/bing.php`

效果：

![jsDelivr 下载资源](3.webp)


---

> 作者:   
> URL: https://blog.wenyi.org/posts/jsdelivr-accelerated-github-resources/  

