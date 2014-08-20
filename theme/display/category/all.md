# 输出全部分类

在任意位置插入代码：

```php
<?php wp_list_categories() ?>
```

就可以看到所有文章的分类。

本节代码 `step06`

---

### 需要解释：

* 如果没有显示全部分类，不妨加个参数试试。像这样：

  ```php
  <?php wp_list_categories(array('hide_empty' => false)) ?>
  ```

* `wp_list_categories` 又是一个WP的全局方法，后期你会发现越来越多的类似方法。

* 对这个方法需要有很多的订制，比如：排序方法、是否显示描述、是否显示分类下文章的数量等，可参考 [官方解释](http://developer.wordpress.org/reference/functions/wp_list_categories/)。

### 需要注意

* 分类和标签的用法非常的类似，但是表现意义上的差别很大，请不要混淆两者。
