## 在自定义的页面中输出文章

对于某一个`页面`，我想为它单独设置一种样式，完全不同于其他文章。该怎么操作呢？

非常好办。

### 1. 在主题目录下创建一个文件 `template-spring-field.php`
```php
<?php
/*
  Template Name: Spring Field Page
 */
?>
<p>This is spring field page.</p>

<?php the_post() ?>
<h2><?php the_title() ?></h2>
<p><?php the_content(); ?></p>
```

### 2. 创建一个Page，标题和内容随意写。在右侧的 ` /页面属性/模板/` 中选择 `Spring Field Page`。保存，查看这个页面。


哈哈，你想要的效果就有了。

本节代码 `step05`

---

#### 需要解释
- 这个文件的文件名，不必以 `template` 开头，只是这样命名的能更明显的把模板类文件区分出来
- 文件内容的开头，必须是这样写的（模板名称写在注释中），你也可以看到，Template Name 就是显示在后台右侧模板选项的内容


##### 需要注意

- 本节介绍的是页面，不是文章，一般情况下只有页面会有这种需求
