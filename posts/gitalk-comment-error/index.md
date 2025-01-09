# Gitalk 评论出错

我昨天发现了一个问题，就是更改了用户名后 Gitalk 评论出错，无法加载评论（**Error: Request failed with status code 403**）。

我认为问题出在了没有重新设置 GitHub Application，使用的还是以前的用户名。后来发现没有这么简单，在网上搜索后看到了这一篇文章。
[https://zhuanlan.zhihu.com/p/350735142](https://zhuanlan.zhihu.com/p/350735142)

**发现了问题：**
**PSA: Public demo server ([http://cors-anywhere.herokuapp.com)](http://cors-anywhere.herokuapp.com)) will be very limited by January 2021, 31st**

_The demo server of CORS Anywhere ([http://cors-anywhere.herokuapp.com)](http://cors-anywhere.herokuapp.com)) is meant to be a demo of this project. But abuse has become so common that the platform where the demo is hosted (Heroku) has asked me to shut down the server, despite efforts to counter the abuse (rate limits in #45 and #164, and blocking other forms of requests). Downtime becomes increasingly frequent (e.g. recently #300, #299, #295, #294, #287) due to abuse and its popularity._

_To counter this, I will make the following changes:_
_1.The rate limit will decrease from 200 (#164) per hour to 50 per hour._
_2.By January 31st, 2021, [http://cors-anywhere.herokuapp.com](http://cors-anywhere.herokuapp.com) will stop serving as an open proxy._
_3.From February 1st. 2021, [http://cors-anywhere.herokuapp.com](http://cors-anywhere.herokuapp.com) will only serve requests after the visitor has completed a challenge: The user (developer) must visit a page at [http://cors-anywhere.herokuapp.com](http://cors-anywhere.herokuapp.com) to temporarily unlock the demo for their browser. This allows developers to try out the functionality, to help with deciding on self-hosting or looking for alternatives._

然后点击这个链接：[https://cors-anywhere.herokuapp.com/corsdemo](https://cors-anywhere.herokuapp.com/corsdemo) 操作就可以了。


---

> 作者:   
> URL: https://blog.wenyi.org/posts/gitalk-comment-error/  

