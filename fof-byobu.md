> 中文社区链接：http://iflarum.cn/1225

# FoF 私人讨论

---------------------------------------------------------------

[Aquote]
原文：https://discuss.flarum.org/d/4762
[/Aquote]

# Byōbu by FriendsOfFlarum
[![lincense](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/FriendsOfFlarumbyobu/blob/master/LICENSE) [![packagist](https://img.shields.io/packagist/v/fof/byobu.svg)](https://packagist.org/packages/fof/byobu) [![downloads](https://img.shields.io/packagist/dt/fof/byobu.svg)](https://packagist.org/packages/fof/byobu) [![openclooective](https://img.shields.io/badge/opencollective-support-blue.svg)](https://opencollective.com/fof)

为您的论坛加入私人讨论功能。允许您或用户创建私人讨论，并选择哪些人可见。

## 目标
- 创建仅指定用户或用户组可见的私人讨论。
- 让私人讨论中的回帖实时显示出来。

## 安装
通过[巴扎市场](https://discuss.flarum.org.cn/d/1214)或手动安装：
```sh
composer require "fof/byobu:*"
```

## 更新
```sh
composer update fof/byobu
php flarum migrate
```

## 配置
在论坛后台的插件选项卡中启用本插件。

确保在权限页面设置私人讨论权限。
- 允许创建私人讨论
- 允许编辑私人讨论的参与成员。

## 支持我们的团队
我们很乐意为每个人提供服务。
为此，我们依靠 [OpenCollective](https://opencollective.com/fof) 的自愿捐助。

## 链接
- [Flarum 国际论坛讨论帖](https://discuss.flarum.org/d/4762-fof-by-bu-well-integrated-advanced-private-discussions)
- [GitHub 源码](https://github.com/FriendsOfFlarum/byobu)
- [更新日志](https://github.com/FriendsOfFlarumbyobu/blob/master/CHANGELOG.md)
- [报告问题](https://github.com/FriendsOfFlarumbyobu/issues)
- [通过 Packagist 下载](https://packagist.org/packages/fof/byobu)

FriendsOfFlarum 扩展程序。

[Aquote]
本译文仅用于学习和交流目的，转载请务必注明文章译者、原文出处、和本文链接。
[/Aquote]

---------------------------------------------------------------------

[Aquote]
发布：[ianm](https://discuss.flarum.org/d/4762/483)
[/Aquote]

### 0.4.2
- 兼容 MySQL 8

### 升级更新

> composer require fof/byobu

---------------------------------------------------------------------

[Aquote]
发布：[ianm](https://discuss.flarum.org/d/4762/495)
[/Aquote]

### 0.4.3
- 增加指定标签功能。设置私人讨论在创建时自动归入的分类标签。
- 当此设置开启时，私人讨论位于首页主题列表、主题页横幅中的标签将会被移除。
- 创建私人讨论的对话框中也会将移除标签选择器。

https://user-images.githubusercontent.com/16573496/75630552-a0b2d600-5be3-11ea-9421-a285ad26d941.png

https://user-images.githubusercontent.com/16573496/75630614-4bc38f80-5be4-11ea-966c-365b133defd4.png

https://user-images.githubusercontent.com/16573496/75630696-e9b75a00-5be4-11ea-8111-535af91fecd5.png

### 升级
> composer require fof/byobu

---------------------------------------------------------------------

[Aquote]
发布：[ianm](https://discuss.flarum.org/d/4762/553)
[/Aquote]

### 0.5.0-beta.1

- 修复编辑用户会导致标签检查失败的问题；
- 允许用户退出私人讨论，并通知其余用户；
- 移除与用户退出讨论有关的通知；
- 删除未使用的翻译键；
- 修复了他人主页点击「发起私人讨论」按钮时不会预先填充收件人的问题；
- 将用户添加到现有私人讨论中时的通知；
- 添加选项以将私人讨论转为公开，并增加权限设置限制可使用此功能的用户组；
- 修复了以下问题：当用户无权点击「发起私人讨论」按钮时，该按钮仍然可见的问题；
- 
[upl-image-preview url=https://flarum.csur.fun/2020-04-04/1586017163-570330-image.png]

[upl-image-preview url=https://flarum.csur.fun/2020-04-04/1586017172-859194-image.png]

[upl-image-preview url=https://flarum.csur.fun/2020-04-04/1586017179-7846-image.png]

[upl-image-preview url=https://flarum.csur.fun/2020-04-04/1586017186-248146-image.png]

[upl-image-preview url=https://flarum.csur.fun/2020-04-04/1586017193-905620-image.png]

由于这是一个重大更新，因此我决定在完全发布它之前运行几次测试版。一如既往地欢迎反馈，请直接在 GitHub 上报告任何问题，以便我可以更好地跟踪它们😉

### 安装
```sh
composer require fof/byobu:0.5.0-beta.1
php flarum cache:clear
```

---------------------------------------------------------------------

[Aquote]
发布：[ianm](https://discuss.flarum.org/d/4762/568)
[/Aquote]

# 0.5.0
没有实质性升级，只是 `0.5.0-beta.1` 已经完成了测试使命。🙂

更新
```
composer require fof/byobu
php flarum cache:clear
```

---------------------------------------------------------------------

[Aquote]
发布：[Askvortsov](https://discuss.flarum.org/d/4762/598)
[/Aquote]

# 0.5.1
Byobu 现在可以导出组件，这样其他扩展就可以使用它们，这个改变是为了给 FoF 草稿增加自动保存功能。

--------------------------------------------------------------------

[Aquote]
发布：[ianm](https://discuss.flarum.org/d/4762/599)
[/Aquote]

# 0.5.1（续）
_是我的错，注释里没写全_

- 增加对「创建私人讨论」和「回复私人讨论」的群组接收者通知的支持。
- 增加「公开私人讨论」的用户接收者通知。
- 一些小的 bug 修复

更新
```
composer require fof/byobu
php flarum cache:clear
```

--------------------------------------------------------------------

[Aquote]
发布：[ianm](https://discuss.flarum.org/d/4762/600)
[/Aquote]

# 0.5.2
- 修复 [giffgaff 社区](https://community.giffgaff.com/) 发现的问题，即从用户卡启动私人讨论时（限制 Byobu 使用指定标签时），仍然需要选择标签。

更新
```
composer require fof/byobu^0.5.2
php flarum cache:clear
```

--------------------------------------------------------------------

[Aquote]
发布：[ianm](https://discuss.flarum.org/d/4762/601)
[/Aquote]

# 0.5.3
今天的有点频繁哈 🙂

- 【移动设备 UI】改进「发起私人讨论」按钮的位置。
- 【移动设备 UI】在选择私人讨论成员模式中增加「取消」按钮。
- 【开发】允许第三方主题根据自己的需要进行定制，包含CSS类 `fof-byobu_primaryControl`。

更新
```
composer require fof/byobu
php flarum cache:clear
```

感谢 [@davwheat](https://discuss.flarum.org/u/davwheat) 的贡献。 👍️

--------------------------------------------------------------------

[Aquote]
发布：[ianm](https://discuss.flarum.org/d/4762/611)
[/Aquote]

# 0.5.4

- 修复从用户资料卡创建私人讨论后，composer 文本编辑器仍处于打开状态的问题 [FriendsOfFlarum/byobu#120](https://github.com/FriendsOfFlarum/byobu/issues/120)。
- 在扩展设置中使用下拉菜单选择要使用的标签。
- 在论坛导航栏中增加显示私人讨论链接的选项（如 [ornanovitch](https://discuss.flarum.org/d/4762/602) 所说）。
- 改进绕过标签的代码（如果启用了选项）。

其他一些[未解决问题](https://github.com/FriendsOfFlarum/byobu/issues)的工作仍在进行中。

更新
```
composer require fof/byobu:^0.5.4
php flarum cache:clear
```

感谢 [@davwheat](https://discuss.flarum.org/u/davwheat) 对 [FriendsOfFlarum/byobu#120](https://github.com/FriendsOfFlarum/byobu/issues/120) 的贡献。 👍️

--------------------------------------------------------------------

[Aquote]
发布：[ianm](https://discuss.flarum.org/d/4762/619)
[/Aquote]

# 0.5.5

- 允许管理员为所有新的私人讨论预先选择一个主要或次要标签（以前只支持主要标签）。(谢谢 [@davwheat](https://discuss.flarum.org/u/davwheat) 的贡献 )
- 修正了在私人讨论中的帖子收到赞或反应时发出的错误「已恢复」通知。[FriendsOfFlarum/byobu#114](https://github.com/FriendsOfFlarum/byobu/issues/114)
- 修复重复回复/发布的通知。[FriendsOfFlarum/byobu#123](https://github.com/FriendsOfFlarum/byobu/issues/123)

更新
```
composer require fof/byobu
php flarum cache:clear
```