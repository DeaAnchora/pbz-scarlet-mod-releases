# 影境转生红莲大人，开局遇见理智孽奇拔

《影之刃零》（PBZ）红莲角色Mod、星刃外观适配，以及迅驰模式。

## 下载

**红莲主包：[V12.0.1 测试版](https://github.com/DeaAnchora/pbz-scarlet-mod-releases/releases/tag/v12.0.1)** · [下载完整ZIP](https://github.com/DeaAnchora/pbz-scarlet-mod-releases/releases/download/v12.0.1/PBZ-Scarlet-v12.0.1-full.zip) · [版本说明](docs/V12.0.1.md)

V12整合旗袍、毛衣、优雅裙装及近期星刃适配。优雅裙装改进了织物光泽、袖子与背部飘带的纱质层次，以及双腿和裙摆的动态避让。默认旗袍，按N依次切换外观。

请下载Release的**附件ZIP**。GitHub自动生成的`Source code (zip)`和`Source code (tar.gz)`只包含仓库文档，不能用于安装Mod。

## 安装

1. 完全退出游戏。
2. 解压完整ZIP，保持全部目录结构。
3. 将解压后的完整Mod文件夹放入PBZ游戏根目录，与`platform`、`ProjectPBZ`文件夹同级，再运行Mod文件夹内的`安装.cmd`。
4. 安装完成后再启动游戏。快捷键可在`快捷键设置.lua`中调整。

```text
影境转生红莲大人，开局遇见理智孽奇拔/
├─ 安装.cmd
├─ 卸载.cmd
├─ 快捷键设置.lua
├─ 说明.txt
└─ Mod文件/
```

包内包含UE4SS运行文件及完整的`Mod文件/UE4SS-FirstInstall/`，无需从旧包补文件。支持首次安装和受支持的V11.2.4升级；使用V12.0.0或其它旧版时，请先使用对应旧包的卸载入口，再安装本版，并保留旧备份与个人配置。安装器会检查已有文件、保留配置并创建备份；遇到冲突提示请保留信息并反馈，不要强制覆盖。

安装与独立回退支持游戏根目录及上级的本地目录联接、符号链接和系统卷挂载入口。游戏内部受管路径单独重定向仍会拒绝；Windows PowerShell5.1过长路径会在写入前提示。

## 本版更新与已知问题

- 红莲外观生效后，暂停已经隐藏的原角色头发、上衣、裙子和披风布料模拟，减少可能的重复计算。
- 保留红莲头发、裙摆、袖子和背部飘带的动态设置，以及现有材质、动画、武器和技能内容。
- 提供完整安装包、UE4SS首次安装文件和独立回退工具。

实际性能收益取决于原布料组件是否启用以及场景负载，尚未完成新版帧时间对照。复杂动作下的衣物避让、部分武器独立技能特效及长期稳定性仍在完善。详细内容见[V12.0.1版本说明](docs/V12.0.1.md)，历史版本见[更新记录](CHANGELOG.md)。

## 迅驰模式（可选）

**[迅驰模式V9.0.9测试版](https://github.com/DeaAnchora/pbz-scarlet-mod-releases/releases/tag/swift-v9.0.9)** · [下载完整ZIP](https://github.com/DeaAnchora/pbz-scarlet-mod-releases/releases/download/swift-v9.0.9/PBZ-Swift-Mode-v9.0.9-full.zip) · [安装与快捷键说明](docs/Swift-Mode-V9.0.9.md)

迅驰是红莲角色的独立附加模块，需要先安装红莲主包。目前支持白旗袍和毛衣外观，默认关闭；按**F10**或同时点按**LB+RB**切换。它单独下载、安装，不会随主包默认启用。

如需显式指定游戏目录，或使用PowerShell 7处理较长路径，请在包含`安装.cmd`的完整包文件夹中打开终端，执行下面的命令。示例路径请替换为自己的PBZ游戏根目录：

```powershell
pwsh -NoProfile -ExecutionPolicy Bypass -File ".\Mod文件\安装管理.ps1" -Action Install -GameRoot "D:\Games\PBZ"
```

## 卸载与回退

退出游戏后运行`卸载.cmd`，或使用本次备份目录中的`回退到安装前.cmd`。V12备份位于游戏根目录`ModBackups/ScarletV12001/`。

回退会恢复安装前文件，并移除本次新增项。请保留完整备份目录；移走安装包后仍可使用备份内的独立入口。文件被手动修改或备份损坏时会停止，避免覆盖改动。

## 校验与反馈

V12完整包`PBZ-Scarlet-v12.0.1-full.zip`的SHA256：

```text
119fbff4bf110a0e1ca8a8c4d45c40609ef296f952aa02ccdf58b39c2418130f
```

Release附件另有`SHA256SUMS.txt`。遇到问题请通过[Issues](https://github.com/DeaAnchora/pbz-scarlet-mod-releases/issues)反馈版本、外观、武器、操作步骤、截图或对应时间的日志。UE4SS原始许可证随包保留。
