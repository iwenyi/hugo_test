# 缓解 WordPress 文章 ID 不连续问题

## 前言

最近浏览小站时，发现最新的一篇文章的 ID 已经是 441 了，小站总共才 30 多篇文章。

查找相关资料后得知，这个问题是自动保存文章版本造成的。WordPress 每次保存草稿的时候，都会在数据库中添加新的记录占用 ID。

决定修改自动保存的频率和限制修订版本最大数量，不完全禁止。

## 修改

解决这个问题有两种修改方法，一个是修改 **WordPress** **wp-config.php** 文件，另一个是修改**主题** **functions.php** 文件。对于这两种方法，我更倾向于选择前者，因为后者在更换主题后需要重新设置，有点麻烦，就不再说了。

### 修改 wp-config.php 文件

自动保存的间隔时间设置为 **120 秒**：

&lt;pre class=&#34;wp-block-zibllblock-enlighter&#34;&gt;&lt;code class=&#34;gl&#34; data-enlighter-language=&#34;generic&#34; data-enlighter-theme=&#34;&#34; data-enlighter-highlight=&#34;&#34; data-enlighter-linenumbers=&#34;&#34; data-enlighter-lineoffset=&#34;&#34; data-enlighter-title=&#34;&#34; data-enlighter-group=&#34;&#34;&gt;//自动保存的间隔时间
define(&#39;AUTOSAVE_INTERVAL&#39;, 120);&lt;/code&gt;&lt;/pre&gt;

修订版本的最大数量设置为 **3 个版本**：

&lt;pre class=&#34;wp-block-zibllblock-enlighter&#34;&gt;&lt;code class=&#34;gl&#34; data-enlighter-language=&#34;generic&#34; data-enlighter-theme=&#34;&#34; data-enlighter-highlight=&#34;&#34; data-enlighter-linenumbers=&#34;&#34; data-enlighter-lineoffset=&#34;&#34; data-enlighter-title=&#34;&#34; data-enlighter-group=&#34;&#34;&gt;//修订版本的最大数量
define(&#39;WP_POST_REVISIONS&#39;, 3);&lt;/code&gt;&lt;/pre&gt;

## 总结

这么做只能缓解 ID 不连续问题，只对修改后新增的文章有效，对修改前的文章无效。


---

> 作者:   
> URL: https://blog.wenyi.org/posts/wordpress-post-id-discontinuity-issue/  

