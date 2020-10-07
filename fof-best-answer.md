> 中文社区链接：http://iflarum.cn/1323

# FoF 最佳回复

---------------------------------------------------------------

[Aquote]
原文：https://discuss.flarum.org/d/21894
[/Aquote]

# Best Answer by [FriendsOfFlarum](https://discuss.flarum.org/d/16242-friends-of-flarum-the-collaboration-for-maintained-extensions)

![license](https://img.shields.io/badge/license-MIT-blue.svg) [![packagist](https://img.shields.io/packagist/v/fof/best-answer.svg)](https://packagist.org/packages/fof/best-answer) [![downloads](https://img.shields.io/packagist/dt/fof/best-answer.svg)](https://packagist.org/packages/fof/best-answer) [![openclooective](https://img.shields.io/badge/opencollective-fof-blue.svg)](https://opencollective.com/fof/donate) [![donate](https://img.shields.io/badge/donate-datitisev-important.svg)](https://datitisev.me/donate)

选择主题中的最佳回复。由 @WiwatSrt 原创。

已改进：

- 修复标签权限问题
- 修复了无法删除最佳回复的问题
- 修复了使用夜间模式时文本太暗的问题。
- 将选择按钮移至更多选项菜单 - 看上去更干净
- 优化主题的最佳答案标志的计算机制
  - 现在仅在讨论页加载最佳回复，在主题_列表中_仅加载一个属性用来表明该主题确实存在最佳回复。
- 支持显示已删除用户的最佳回复显示 & 优化发布速度（希望）

### 截图
>! - 设为最佳回复按钮
> https://s1.ax1x.com/2020/08/22/dUt9LF.png
> - 最佳回复效果
> https://s1.ax1x.com/2020/08/22/dUtEJ1.png
> - 插件设置
> https://s1.ax1x.com/2020/08/22/dUt7Sx.png

### 安装
通过[巴扎市场](https://discuss.flarum.org.cn/d/1214)或 composer 手动安装：
```
composer require fof/best-answer
```

### 更新
```
composer update fof/best-answer
```

### 链接
[![OpenCollective](https://img.shields.io/badge/donate-friendsofflarum-44AEE5?style=for-the-badge&logo=open-collective)](https://opencollective.com/fof/donate) [![GitHub](https://img.shields.io/badge/donate-datitisev-ea4aaa?style=for-the-badge&logo=github)](https://datitisev.me/donate/github)
- [国际社区讨论帖](https://discuss.flarum.org/d/21894)[ext]
- [Packagist](https://packagist.org/packages/fof/best-answer)
- [GitHub](https://github.com/FriendsOfFlarum/best-answer)
- [Wiwatsrt's Best Answer](https://packagist.org/packages/sijad/flarum-ext-best-answer)

[FriendsOfFlarum](https://github.com/FriendsOfFlarum) 制作扩展。

[Aquote]
本译文仅用于学习和交流目的，转载请务必注明文章译者、原文出处、和本文链接。
[/Aquote]



---------------------------------------------------------------------

[Aquote]
发布：[ianm](https://discuss.flarum.org/d/21894/43)
[/Aquote]

### 0.1.7

- 当用户将自己的帖子选为最佳回复时，不推送通知
- 使用队列推送通知
- 新增「我参与的讨论有最佳回复」通知订阅功能 - 默认关闭

### 更新
```
composer require fof/best-answer
php flarum cache:clear
```

---------------------------------------------------------------------

[Aquote]
发布：[ianm](https://discuss.flarum.org/d/21894/51)
[/Aquote]

# 0.1.8
🚨 跨主题讨论漏洞

此版本解决了今天发现的一个问题，即使用户没有权限通过 REST API 查看该帖子或讨论，也可以从另一个讨论中设置最佳答案。

我强烈建议尽快从以前的任何版本进行更新。

### 更新
```
composer require fof/best-answer:^0.1.8
php flarum cache:clear
```

---------------------------------------------------------------------

[Aquote]
发布：[ianm](https://discuss.flarum.org/d/21894/53)
[/Aquote]

# 0.1.9
- 解决手机上的格式问题，谢谢 [rafaucau](https://github.com/rafaucau)！

### 更新
```
composer require fof/best-answer:^0.1.9
php flarum cache:clear
```

---------------------------------------------------------------------

[Aquote]
发布：[ianm](https://discuss.flarum.org/d/21894/61)
[/Aquote]

# 0.1.10
- 修复了设置最佳答案后立马取消最佳答案时的通知同步错误。

### 更新
```
composer require fof/best-answer:^0.1.10
php flarum cache:clear
```