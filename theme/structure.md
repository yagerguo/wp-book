## 主题的文件结构

主题的文件结构的是开发主题之前的预备知识，必须要明白。

### 最基本

最简单的主题只需要一个 `index.php` 就够了。

### 再细分

可以分为三种

1. 首页 `index.php` ，类似于 [爱彩雲首页](http://www.icaiyun.com/) , 完全的自定义
2. 文章页 `single.php`，类似于 [WP生态链](http://www.icaiyun.com/wordpress-life.html) ，单单的是有一篇文章
3. 文章列表页 `category.php` ，类似于 [学好WP](http://www.icaiyun.com/category/learn-wordpress) ，是一大批跟WP有关的文章

### 还可以再细分

- 单页 `page.php` ，类似于 [给我留言](http://www.icaiyun.com/message)，孤立的一个页面，不属于任何分类
- 按筛选条件不同，文章列表页可以分为
  * 按日期 `archive.php`
  * 按作者 `author.php`
  * 按标签 `tag.php`
  * 按内容 `search.php` ，其实也就是搜索

### 其他文件

- `header.php` 通常开发都会把头部和底部分离出来，WP也一样
- `footer.php`
- `functions.php` 用来存放一些主题需要用到的自定义方法

----

当然WP的主题文件也不止这些，有些还可以更加细分。有了这些基本就够用了，后边用到了我们会再次去讲。
