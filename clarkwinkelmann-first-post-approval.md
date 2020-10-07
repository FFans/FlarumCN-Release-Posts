[Aquote]
原文：https://discuss.flarum.org/d/25055
作者：[Clarkwinkelmann](https://discuss.flarum.org/u/clarkwinkelmann)
[/Aquote]

# First Post Approval

[![MIT license](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/clarkwinkelmann/flarum-ext-first-post-approval/blob/master/LICENSE.md) [![Latest Stable Version](https://img.shields.io/packagist/v/clarkwinkelmann/flarum-ext-first-post-approval.svg)](https://packagist.org/packages/clarkwinkelmann/flarum-ext-first-post-approval) [![Total Downloads](https://img.shields.io/packagist/dt/clarkwinkelmann/flarum-ext-first-post-approval.svg)](https://packagist.org/packages/clarkwinkelmann/flarum-ext-first-post-approval) [![Donate](https://img.shields.io/badge/paypal-donate-yellow.svg)](https://www.paypal.me/clarkwinkelmann)

通过本扩展为所有用户设置「无需审核即可发帖」的前置审核额度。

使用本扩展，可以有效治理垃圾信息的侵扰，基本防治理念为：全新的垃圾账号注册后，在使用完前置审核额度前，其发布的内容都会被送入审核队列，不予立即公开，这样可以消灭垃圾内容在无监管时的长时间曝光。

您可以在权限页面指定用户组不受本扩展约束。

当一个回复帖被批准后，回帖前置审核计数会 +1。

当一个主题帖被批准后，主题前置审核计数会 +1，同时回帖前置审核计数也会 +1。

如果您没有设置主题前置审核额度，则计数会基于回帖前置审核额度。

比如，如果您设置回帖前置审核额度为 2，主题审核额度为0，则当用户在本插件第一次启用后，发布的两条内容之一包含主题帖时，该主题帖会被送入审核队列。
如果该用户在审核额度生效后，发布的两条内容均是回帖后，则在他发布第一个主题帖（第三条内容）时，该主题帖无需审核即可顺利发表。

### 现有用户

如果您的论坛已经拥有了用户，您需要手动修改数据库 `user` 表中每位用户的 `first_post_approval_count` 和 `first_discussion_approval_count` 列（字段/属性） 的值，以使这些用户不受本扩展的约束。

将上述属性的值设置为：任何等于或大于您设置的前置审核额度的数字，即可使这些用户不受约束。

您也可以在权限页面设置某些用户组不受约束。

### 安装

安装前，必须先启用 Flarum 的 **审核** 及 **标签** 插件。

```
composer require clarkwinkelmann/flarum-ext-first-post-approval
```

### 支持

本扩展所需的维护不多。

本扩展是为一个客户开发的，并以开源的形式发布，以造福社区。

作者可能会免费发布简单的错误修复或兼容性更新。

您可以[联系作者](https://clarkwinkelmann.com/flarum)赞助额外的功能或更新。

作者将在 [Flarum 国际社区讨论帖](https://discuss.flarum.org/d/25055)以「尽力而为」的方式提供支持。

[Aquote]
本译文仅用于学习和交流目的，转载请务必注明文章译者、原文出处、和本文链接。
[/Aquote]