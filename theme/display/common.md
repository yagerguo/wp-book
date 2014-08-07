# 输出网站基本信息

废话不多说，直接开始敲代码

#### 1. 在 `header.php` 中这样写
```html
<html>
    <head>
        <title><?php bloginfo('name'); ?></title>
    </head>
    <body>
```

#### 2. 在 `footer.php` 中这样写
```html
    </body>
</html>
```

#### 3. 在 `index.php` 中引入 `header.php` 和 `footer.php`
```php
<?php
get_header();
echo 'Hello, welcome to ';
bloginfo('name');
echo ' !';
get_footer();
?>
```

#### 好了，这样就可以输出网站标题了。
本节代码 `setp02`

----

解释下其中的几个方法：

- `bloginfo()` 方法可以获取博客全局的一些信息，比如：标题、关键字、全局样式等，[详细使用说明](http://developer.wordpress.org/reference/functions/bloginfo/
)。
- `get_header()` 和 `get_footer()` 用来引入 `header.php` 和 `footer.php`

你可能会问：

- 如何输出自定义内容，如网站版权信息、统计代码、自定义广告代码等。你可以在后边的文章中找到答案。

