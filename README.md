# Rynoa 1.0.0 (2) — 测试版

Rynoa 是 macOS 菜单栏快捷动作工具，可将右 Command、右 Option 和机身拍击绑定到常用应用、快捷键或系统动作。

- 右 Command / 右 Option 支持双击、三击和长按。
- 机身拍击支持双击、三击和四击，不区分左右，单击不触发。
- 支持暂停触发、动作提示和本地保存配置。
- 传感器按需运行，异常中断自动尝试恢复。

## 下载与安装

[下载测试版 DMG](https://github.com/JinSooo/rynoa-releases/releases/download/v1.0.0-beta.2/Rynoa-1.0.0-beta.2.dmg) · [SHA-256 校验文件](https://github.com/JinSooo/rynoa-releases/releases/download/v1.0.0-beta.2/Rynoa-1.0.0-beta.2.dmg.sha256) · [全部版本](https://github.com/JinSooo/rynoa-releases/releases)

下载两个文件到同一目录后，可运行：

```sh
shasum -a 256 -c Rynoa-1.0.0-beta.2.dmg.sha256
```

打开安装包，把 Rynoa 拖入 Applications，再从 Applications 启动。按设置页指引授予对应输入监控/辅助功能权限，配置动作后使用。建议先用打开应用等容易确认的动作测试。

## 适用范围

macOS 14 或更新版本。应用包含 Apple Silicon 与 Intel 架构，但机身拍击只在当前开发机完成验证；包含架构不代表对应硬件有可用的拍击传感器。

机身拍击依赖机器内部传感器及未公开接口，其他 Mac 型号、系统更新和桌面条件仍需验证。弱拍击可能漏检，桌面冲击可能误检。请先试用确认，轻柔敲击即可。

此包为 Apple Development 开发签名，尚未完成 Developer ID 发行签名与 Apple 公证，系统可能阻止打开。正式公证包准备好后另行发布。

## 收费状态

当前构建没有付费授权或试用到期限制，支付尚未开放。后续收费版的售价、试用规则和授权范围会单独公布。

## 反馈

反馈时请注明 macOS 版本、Mac 型号、触发方式及复现步骤。无需提供许可证、个人配置文件或原始键盘输入。

本仓库只提供发行说明、安装包和反馈入口。[提交问题](https://github.com/JinSooo/rynoa-releases/issues/new)；请勿在公开反馈中提交个人信息。
