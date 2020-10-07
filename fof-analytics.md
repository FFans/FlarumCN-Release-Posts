> 中文社区链接：http://iflarum.cn/1943

# FoF 访客统计

[Aquote]
原文：https://discuss.flarum.org/d/1983
[/Aquote]

# FriendsOfFlarum Analytics
[![MIT license](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/FriendsOfFlarum/analytics/blob/master/LICENSE.md) [![Latest Stable Version](https://img.shields.io/packagist/v/fof/analytics.svg)](https://packagist.org/packages/fof/analytics) [![Total Downloads](https://img.shields.io/packagist/dt/fof/analytics.svg)](https://packagist.org/packages/fof/analytics) [![OpenCollective](https://img.shields.io/badge/opencollective-fof-blue.svg)](https://opencollective.com/fof/donate)

[Flarum](http://flarum.org/) 扩展程序。为您的社区提供谷歌统计、Piwik 统计功能。

### 截图
- 谷歌统计
![截图](https://s1.ax1x.com/2020/08/21/dNsTw6.png)
- Piwik 统计
![截图](https://s1.ax1x.com/2020/08/21/dNyu7V.png)
![截图](https://s1.ax1x.com/2020/08/21/dNytn1.png)

### 安装
使用 [巴扎市场](https://discuss.flarum.org.cn/d/1214) 或通过 composer 手动安装：
```
composer require fof/analytics
```

### 配置

- Piwiki 的网址不能以 '/' 结尾，正确的格式如：domain.com 或 domain.com/piwik
- 访问后台管理面板的扩展选项卡来配置你的统计服务。
- 访问后台管理面板的 Analytics 选项卡，查看 piwik 的分析结果。

### 链接

- [Flarum 国际社区讨论帖](https://discuss.flarum.org/d/1983)
- [GitHub 源代码](https://github.com/FriendsOfFlarum/analytics)
- [报告问题](https://github.com/FriendsOfFlarum/analytics/issues)
- [通过 Packagist 下载](https://packagist.org/packages/fof/analytics)

[FriendsOfFlarum](https://friendsofflarum.org/) 扩展程序。

[Aquote]
本译文仅用于学习和交流目的，转载请务必注明文章译者、原文出处、和本文链接。
[/Aquote]

---------------------------------------------------------------------

[Aquote]
发布：[ianm](https://discuss.flarum.org/d/1983/194)
[/Aquote]
## 0.9.0

- 从 Flagrow 迁移到 FoF 命名空间，**请看下面的升级说明**。
- 增加了对 Google Optimize 和/或 GTM 的支持（感谢 [giffgaff](https://community.giffgaff.com/)）

### 更新

```
composer require fof/analytics
php flarum migrate
php flarum cache:clear
```

Composer _应该_ 会自动删除 `flagrow/flarum-ext-analytics`，然后用新版本替换。如果因为某些原因没有这样，请使用 `composer` 删除旧软件包。

不要忘了启用扩展，因为一开始它会被禁用。

---------------------------------------------------------------------

[Aquote]
发布：[ianm](https://discuss.flarum.org/d/1983/207)
[/Aquote]

## 0.9.1

- 修复仅提供/启用谷歌跟踪代码时出现的问题（[@rossoblu/201](https://discuss.flarum.org/d/1983/201)）

### 更新

```
composer require fof/analytics:^0.9.1
php flarum cache:clear
```