# 影境转生红莲大人，开局遇见理智孽奇拔

《影之刃零》（PBZ）红莲角色Mod、可选的迅驰模式。

## 下载

**红莲主包：[V11.1.3 测试版](https://github.com/DeaAnchora/pbz-scarlet-mod-releases/releases/tag/v11.1.3)** · [下载完整ZIP](https://github.com/DeaAnchora/pbz-scarlet-mod-releases/releases/download/v11.1.3/-v11.1.3.zip) · [版本说明](docs/V11.1.3.md)

本版包含黑伤LB+Y强化红光的星刃适配，并新增黑伤LT独立特效适配。LT贴合效果、其它武器的部分技能特效和持续战斗稳定性仍在测试、完善中。

请下载Release的**附件ZIP**。GitHub自动生成的`Source code (zip)`和`Source code (tar.gz)`仅包含仓库文档，不能用来安装Mod。

## 安装

1. 完全退出游戏。
2. 解压完整ZIP，保持目录结构，不要只提取其中几个文件。
3. 运行`安装.cmd`，按提示选择PBZ游戏根目录。
4. 安装完成后再启动游戏。

安装包结构如下：

```text
影境转生红莲大人，开局遇见理智孽奇拔/
├─ 安装.cmd
├─ 卸载.cmd
├─ 快捷键设置.lua
├─ 说明.txt
└─ Mod文件/
```

包内已包含UE4SS运行文件和完整的`Mod文件/UE4SS-FirstInstall/`，不需要从旧包补文件。快捷键设置见`快捷键设置.lua`。

V11.1.3支持首次安装，以及从受支持的V11.1.2安装升级。安装器会检查完整性、游戏状态和已有文件，并保存安装前备份；你的快捷键配置和其它Mod会按安装规则保留。如果提示版本或文件不匹配，请保留提示信息并反馈，不要强制覆盖。

## 本版更新

- 黑伤LB+Y强化红光适配星刃刀身。
- 新增黑伤LT红黑特效的独立空间适配，保留原特效和技能时序。
- 保留动画与特效回调隔离、收拔刀和过场后的武器恢复处理。
- 继续逐项完善其它武器的技能特效，尚未覆盖所有独立特效。

详细变化及已知问题见[V11.1.3版本说明](docs/V11.1.3.md)；历史版本见[更新记录](CHANGELOG.md)。

## 迅驰模式（可选）

**[迅驰模式V9.0.9测试版](https://github.com/DeaAnchora/pbz-scarlet-mod-releases/releases/tag/swift-v9.0.9)** · [下载完整ZIP](https://github.com/DeaAnchora/pbz-scarlet-mod-releases/releases/download/swift-v9.0.9/PBZ-Swift-Mode-v9.0.9-full.zip) · [安装与快捷键说明](docs/Swift-Mode-V9.0.9.md)

迅驰是红莲角色的独立附加模块，需要先安装红莲主包。目前支持白旗袍和毛衣外观，默认关闭；按**F10**或同时点按**LB+RB**切换。它单独下载、安装，不会随主包默认启用。

## 卸载与回退

完全退出游戏后运行`卸载.cmd`，或运行本次备份目录中的`回退到安装前.cmd`。红莲V11.1.3的备份保存在游戏根目录`ModBackups/ScarletV11103/`下。

回退会恢复本次安装前的文件，并移除本次新增内容。请保留备份目录；即使移走原安装包，仍可使用备份内的独立回退入口。如果文件被手动修改或备份损坏，回退会停止，避免覆盖你的改动。

## 校验与问题反馈

Release提供`SHA256SUMS.txt`。V11.1.3完整包的SHA256为：

```text
076bc168143cf5ca20efb41ba1ea9728d1597949aeb2caeb3cf40ce7d16c4add
```

GitHub可能将中文附件名显示为`-v11.1.3.zip`，两者是同一个文件，内容和SHA256不变；校验时请以该版本校验文件中记录的文件名为准。

遇到问题请通过[Issues](https://github.com/DeaAnchora/pbz-scarlet-mod-releases/issues)反馈，附上版本号、武器名称、技能或按键、复现步骤，以及截图或相关日志。崩溃、卡死和过场后异常，请一并说明发生时间。

所有当前发布均为测试版，仍可能出现特效错位、武器显示异常、卡顿或崩溃。我会继续根据反馈修复。UE4SS原始许可证随安装包保留。
