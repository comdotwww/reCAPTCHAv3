[typecho][1]评论验证码插件，使用Google的[reCAPTCHAv3][2]接口。
======

#### 使用方法：
1. 到「[页面][3]」申请一个API key【一定是v3版本的！】；
2. 激活该插件，并配置Public Key和Private Key；
3. 在适当地方添加如下代码：

```
<?php reCAPTCHAv3_Plugin::output(); ?>
```
**注意：若未配置Public Key和Private Key而在页面中先添加上述代码，该页面会报错**

## 可能需要添加的地方
1. 主题模板中的comments.php文件，在评论的表单位置也就是`comments`的`form`标签之间的任何你认为合适的地方，加上代码，如`<button type="submit" class="submit">，`上面加一行

[1]: http://typecho.org/about
[2]: https://www.google.com/recaptcha/
[3]: https://www.google.com/recaptcha/admin/create
