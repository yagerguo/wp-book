## 在单页中输出文章信息

在上一节生成的页面中，细心的你会发现，点击文章标题链接一以后，显示的还是文章列表，应该是显示文章详细页的。本节就来解决这个问题。

跟文章页相关的文件是 `single.php` ,今天就来把他修改成

```php
<?php get_header(); ?>

<?php the_post() ?>
<h2><?php the_title() ?></h2>
<p> This is single page. <?php the_excerpt(); ?></p>

<?php get_footer(); ?>
```

OK，大功告成，就这么简单。

本节代码 `step04`

---

#### 需要解释

- 单页其实也是循环输出，只是只有一个循环罢了，所以 while是省去的，但 the_post() 是不可缺少的。
