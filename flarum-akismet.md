# Akismet 垃圾留言过滤器

Akismet 是 WordPress 较常用的一款防垃圾留言插件。这款强大的插件自 Flarum-beta 3 开始，由 Flarum 官方移植并维护。

### 安装

```
composer require flarum/akismet
```

### 准备工作

- 科学上网工具（需要登录 wordpress.com 以及 Google 验证）；
- WordPres 账号。

### API 申请

个人可以免费申请 Akismet API 密钥，当然也有收费的高级订阅项。

1. 打开 Akismet 官网，登录 WordPress 账号；
　
![步骤一](https://flarum.csur.fun/2020-04-12/1586667594-439644-image.png)

2. 选择免费计划；
　
![步骤二](https://flarum.csur.fun/2020-04-12/1586667648-784404-image.png)

3. 价格拉到 0 元，然后点击继续；
　
![步骤三](https://flarum.csur.fun/2020-04-12/1586667852-492564-image.png)

4. 复制 API KEY 至 Flarum 插件。
　
![步骤四](https://flarum.csur.fun/2020-04-12/1586667896-400184-image.png)

# 误杀处理方法
对于被误杀的帖子，最好不要点击「不是垃圾内容」。如果点了这个，可能会影响以后类似内容的过滤效果。

可以点击「撤销举报」，然后右下角三个点，选择「通过审核」。

![截图一](https://flarum.csur.fun/2020-04-13/1586787811-576860-image.png)

![截图二](https://flarum.csur.fun/2020-04-13/1586787846-285937-image.png)

[Aquote]
这里邀请 @GuguguBear 登场举个栗子，绝无恶意！
[/Aquote]

Flarum [i18n 计划](https://github.com/Flarum-i18n/extension-release-posts-zh-cn)。