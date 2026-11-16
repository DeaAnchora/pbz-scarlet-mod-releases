# 影境转生红莲大人，开局遇见理智孽奇拔

《影之刃零》（PBZ）红莲角色Mod、迅驰模式。

## 下载

**红莲主包：[V11.1.7 测试版](https://github.com/DeaAnchora/pbz-scarlet-mod-releases/releases/tag/v11.1.7)** · [下载完整ZIP](https://github.com/DeaAnchora/pbz-scarlet-mod-releases/releases/download/v11.1.7/-v11.1.7.zip) · [版本说明](docs/V11.1.7.md)

本版补充乱萤鸣剑／双剑强化的右手星刃附刃特效，保留左手天邈、黑伤、冰火与风雷的既有适配。安装器支持本地目录联接、符号链接和系统卷挂载入口。其它武器部分独立特效、持续战斗稳定性和性能尖峰仍在完善中。

请下载Release的**附件ZIP**。GitHub自动生成的`Source code (zip)`和`Source code (tar.gz)`仅包含仓库文档，不能用来安装Mod。

## 安装

1. 完全退出游戏。
2. 解压完整ZIP，保持目录结构，不要只提取其中几个文件。
3. 将解压后的完整Mod文件夹放入PBZ游戏根目录，与`platform`、`ProjectPBZ`文件夹同级，再运行Mod文件夹内的`安装.cmd`。
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

V11.1.7支持首次安装，以及从受支持的V11.1.6安装升级。安装器会检查完整性、游戏状态和已有文件，并保存安装前备份；你的快捷键配置和其它Mod会按安装规则保留。如果提示版本或文件不匹配，请保留提示信息并反馈，不要强制覆盖。

## 本版更新

- 黑伤LB+Y强化红光适配星刃刀身。
- 新增黑伤LT红黑特效的独立空间适配，保留原特效和技能时序。
- 保留动画与特效回调隔离、收拔刀和过场后的武器恢复处理。
- 继续逐项完善其它武器的技能特效，尚未覆盖所有独立特效。

详细变化及已知问题见[V11.1.7版本说明](docs/V11.1.7.md)；历史版本见[更新记录](CHANGELOG.md)。

## 迅驰模式（可选）

**[迅驰模式V9.0.9测试版](https://github.com/DeaAnchora/pbz-scarlet-mod-releases/releases/tag/swift-v9.0.9)** · [下载完整ZIP](https://github.com/DeaAnchora/pbz-scarlet-mod-releases/releases/download/swift-v9.0.9/PBZ-Swift-Mode-v9.0.9-full.zip) · [安装与快捷键说明](docs/Swift-Mode-V9.0.9.md)

迅驰是红莲角色的独立附加模块，需要先安装红莲主包。目前支持白旗袍和毛衣外观，默认关闭；按**F10**或同时点按**LB+RB**切换。它单独下载、安装，不会随主包默认启用。

如需显式指定游戏目录，或使用PowerShell 7处理较长路径，请在包含`安装.cmd`的完整包文件夹中打开终端，执行下面的命令。示例路径请替换为自己的PBZ游戏根目录：

```powershell
pwsh -NoProfile -ExecutionPolicy Bypass -File ".\Mod文件\安装管理.ps1" -Action Install -GameRoot "D:\Games\PBZ"
```

## 卸载与回退

完全退出游戏后运行`卸载.cmd`，或运行本次备份目录中的`回退到安装前.cmd`。红莲V11.1.7的备份保存在游戏根目录`ModBackups/ScarletV11107/`下。

回退会恢复本次安装前的文件，并移除本次新增内容。请保留备份目录；即使移走原安装包，仍可使用备份内的独立回退入口。如果文件被手动修改或备份损坏，回退会停止，避免覆盖你的改动。

## 校验与问题反馈

Release提供`SHA256SUMS.txt`。V11.1.7完整包的SHA256为：

```text
2220f057456eff86b731df5edaf9bec29abd662df27dff86987bf36d2ddc1a1a
```

GitHub可能将中文附件名显示为`-v11.1.7.zip`，两者是同一个文件，内容和SHA256不变；校验时请以该版本校验文件中记录的文件名为准。

遇到问题请通过[Issues](https://github.com/DeaAnchora/pbz-scarlet-mod-releases/issues)反馈，附上版本号、武器名称、技能或按键、复现步骤，以及截图或相关日志。崩溃、卡死和过场后异常，请一并说明发生时间。

所有当前发布均为测试版，仍可能出现特效错位、武器显示异常、卡顿或崩溃。我会继续根据反馈修复。UE4SS原始许可证随安装包保留。
