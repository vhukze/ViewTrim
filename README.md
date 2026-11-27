# 界律 · ViewTrim

界律是一款通用 LSPosed 模块，支持点选并移除 Android 应用中的原生界面控件和部分 Flutter 列表或网格项。

## 安装与使用

需要 Android 9 或更高版本，以及兼容 libxposed API 102 的 LSPosed 环境。包名为 `io.github.vhukze.viewtrim`。

1. 从 [GitHub Releases](https://github.com/vhukze/ViewTrim/releases/latest) 下载并安装 APK，然后在 LSPosed 中启用界律。
2. 打开界律，在应用列表中为目标应用授予作用域。首次授权后，如果目标应用已在运行，请先强行停止它。
3. 从界律点「编辑」启动目标应用。进入目标页面后，点工具条的「选择」，再点要移除的控件。可以通过「扩大范围」或「缩小范围」调整选区。
4. 点「移除所选」保存规则，点「完成」退出编辑。只要目标应用仍在模块作用域内，日常打开应用时就会自动应用规则。

在规则页可以查看控件截图、暂停或删除规则。在设置页可以按应用导入或导出规则和截图。

## 兼容范围

- Flutter 规则在目标应用重开后生效，适用于能唯一定位的列表和网格项。

- 支持能稳定识别的 Android 原生 View。应用更新或页面结构变化后，部分规则可能需要重新选取。
- 支持的布局会自动补位，复杂布局可能留白。
- Compose、自绘界面和网页的内部元素目前无法单独选取。移除发生在界面绘制前，应用仍可能创建控件、执行相关业务或发送网络请求。

## 社区与反馈

- [提交问题](https://github.com/vhukze/ViewTrim/issues)
- [Telegram 频道](https://t.me/vhukze_ViewTrim)
- [Telegram 群组](https://t.me/ViewTrim)

公开仓库提供安装包、使用说明和问题反馈。
