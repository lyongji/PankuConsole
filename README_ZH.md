
# Panku Console 中文说明文档

![logo](./docs/assets/logo.png)

---

**Panku Console 是一个功能丰富的 Godot 引擎实时调试工具包。** 使用 Panku Console，您可以轻松地在运行时与您的脚本和对象进行交互，无论是作弊、调试、原型设计，还是只是想玩得开心 😄🎮。

Panku Console 被设计为模块化和可扩展的，添加和维护功能非常容易。它也被设计得尽可能不干扰，所以您可以在项目中使用它而不用担心对最终产品的影响 🧩🚀。

# ✨ 高光

## 📦 轻量级 - 小于 256KB！

Panku Console 将始终尽可能轻量。

## 🖼️ 多窗口 UI - 按照您想要的布局排列！

任何窗口都可以缩放、吸附、折叠、拖动，甚至可以变成一个[独立的操作系统窗口](./docs/faq.md)。

![ui](./docs/assets/ui.png)

## 💻🔮 [开发者控制台](./docs/developer_console.md) - 在运行时执行任意代码，并带有提示！

允许您在运行时执行任意[表达式](https://docs.godotengine.org/en/stable/tutorials/scripting/evaluating_expressions.html)（例如函数调用），就像您是神一样 🧙‍♂️。

![console](./docs/assets/console.png)

## 📝🕹️ [原生记录器](./docs/native_logger.md) - 在您的游戏中显示原生日志！

在覆盖层或单独的窗口中查看原生日志（与编辑器输出面板相同）📋。

![logger](./docs/assets/logger.png)

## 🛠️🔧 [数据控制器](./docs/data_controller.md) - 将任何对象转换为可调整属性的属性面板！

自动将脚本中的所有导出属性转换为检查器窗口。

![data_controller](./docs/assets/data_controller.png)

## 👀🎮 [表达式监视器](./docs/expression_monitor.md)

在游戏中监视[表达式](https://docs.godotengine.org/en/stable/tutorials/scripting/evaluating_expressions.html)的结果。

![expression_monitor](./docs/assets/expression_monitor.png)

## 还有更多... 🌟

- [历史管理器](./docs/history_manager.md): 查看历史输入。⏪
- [键盘快捷键](./docs/keyboard_shortcut.md): 将表达式绑定到键以快速作弊。⌨️🕹️
- [屏幕通知器](./docs/screen_notifier.md): 在屏幕上显示弹出消息。💬📢
- [纹理查看器](./docs/texture_viewer.md): 实时查看纹理。🖼️👁️
- [杂项命令](./docs/misc_commands.md): 提供一些有用的命令。🛠️🔧
- [常规设置](./docs/general_settings.md): 根据您的喜好自定义控制台。⚙️🔧
- [常见问题](./docs/faq.md): 常见问题。🙋‍♂️🙋‍♀️

由于 Panku Console 是模块化的，您可以轻松地添加或删除功能以适应您的需求。🧩🔧

![modular](./docs/assets/modular.png)

# 安装 🚀

## A. 直接从 GitHub `master` 分支下载

1. 从 Github 下载 [最新提交](https://github.com/Ark2000/PankuConsole/archive/refs/heads/master.zip) 📥。
2. 将 `addons` 文件夹复制到您的项目根目录 📂。
3. 在 Godot 设置中启用此插件 ⚙️: `项目 > 项目设置 > 插件`

## B. 使用镜像仓库作为 git 子模块

或者，如果您更喜欢使用 git（推荐），您可以将此 [镜像仓库](https://github.com/Ark2000/panku_console) 添加为您的 `addons` 文件夹中的子模块，这样在您拉取最新更改时，插件会自动更新 🔄。

```bash
# 在您的项目根目录中
cd addons
git submodule add https://github.com/Ark2000/panku_console
```

## C. 从 [Godot 资源库](https://godotengine.org/asset-library/asset/1558) 下载

这与下载 `godot4_asset_library` 分支相同（始终指向最新的稳定版本，并且只包含 `addons` 文件夹）

---

有关插件安装的更多信息，您可以访问相应的 [Godot 文档 📚](https://docs.godotengine.org/en/stable/tutorials/plugins/editor/installing_plugins.html)。

> **注意**：Panku Console 当前仅支持 Godot 版本 4.x，3.x 支持仍在进行中。

# 贡献 🤝

您想贡献吗？在[贡献部分](./CONTRIBUTING.md)了解更多信息。🌟🙌

此外，请参阅[项目路线图](https://github.com/Ark2000/PankuConsole/discussions/152)以获取更多关于开发计划的详细信息。

# 许可证 📜

[MIT 许可证](./LICENSE)

版权所有 (c) 2022-present, Feo (k2kra) Wu
