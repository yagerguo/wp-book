## 显示评论框

怎么在文章的底部显示评论表单呢？

###1.创建新文件
在主题根目录下创建文件 `comments.php` ，内容

```html
<h3>Comment</h3>
<p><?php comment_form(); ?></p>
```

###2.修改文章页
在 `single.php` 中你觉得合适的地方添加代码

```php
comments_template('', true);
```
###3.完成

是不是意犹未尽的就结束了？看看效果吧。

本节代码和下一小节的代码都在 `step09`
