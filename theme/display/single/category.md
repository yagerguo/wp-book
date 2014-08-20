## 在列表中显示文章

非常的容易。

只需在 `index.php` 的 `get_header()` 和 `get_footer()` 中加入下边的代码就可以了。

```php
<?php while ( have_posts() ) : the_post() ?>

<h2><a href="<?php the_permalink() ?>"><?php the_title() ?></a></h2>
 <p><?php the_excerpt(); ?></p>

<?php endwhile; ?>
```

刷新首页是不是就能看到最新的几篇文章？很容易。

本节代码 `step03`

---

#### 需要解释

- 在列表页中，文章是以循环的方式输出的。具体到每一篇文章的内容，都在循环体 while 内输出。
- 在循环体内可以非常方便的获取单篇文章的信息。
  * `the_title()` 是标题
  * `the_excerpt()` 是摘要
  * `the_permalink()` 是文章链接
  * 在 `/wp-includes/post-template.php` 中可以看到完整的方法列表

