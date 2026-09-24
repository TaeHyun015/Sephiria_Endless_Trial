# Sephiria Endless Trial

[한국어](README.md) | [English](README.en.md) | [日本語](README.ja.md) | [简体中文](README.zh-CN.md)

**Endless Trial** 是 Sephiria 的非官方试炼模组。玩家可以在独立的试炼战斗区域逐关挑战，并且每通关五关前往商人和奖励区域。

以下下载和安装说明适用于 Windows 版 Steam 游戏。[v1.0.0 发布说明（韩语）](RELEASE_NOTES_v1.0.0.md)

## 下载与安装

1. 从[最新版本](https://github.com/TaeHyun015/Sephiria_Endless_Trial/releases/latest)下载 **`Endless_Trial.zip`**。
2. 完全退出游戏。
3. 将 ZIP 解压到 Sephiria 安装目录下的 `AddOns` 文件夹。最终目录结构应如下所示：

   ```text
   Sephiria/
   └─ AddOns/
      └─ Endless_Trial/
         ├─ Endless_Trial.dll
         ├─ endless_trial_floor
         ├─ metadata.json
         └─ Endless_Trial/
            └─ trial_bg.png
   ```

4. 启动游戏。手动更新已有版本时，也请先退出游戏，再将新 ZIP 解压到同一位置并覆盖旧文件。

ZIP 中已经包含 `Endless_Trial` 文件夹。请将其解压到 `AddOns`，不要解压到 `AddOns/Endless_Trial`，以免多出一层同名文件夹。

## 玩法

- 在多人区域的试炼入口传送门处，由房主选择存档栏位进入。多人游戏时，所有玩家都必须聚集在入口附近。
- 与试炼石碑互动以开始关卡。关卡进行期间，试炼战斗区域会播放片尾制作人员名单的背景音乐。
- 每通关五关，通往商人和奖励区域的传送门就会开启。所有玩家返回战斗区域后，才能开始下一关。
- 使用“保存并返回”传送门保存进度并离开。试炼共有三个存档栏位；多人游戏的存档由房主管理。

## 自动更新

发布新版本后，游戏启动时会显示更新确认窗口。接受更新后，模组会下载该版本的 `Endless_Trial.zip`、校验 SHA256 哈希值，并在游戏关闭后替换模组文件、重新启动游戏。取消更新则可以继续使用当前版本游玩。

要让自动更新识别新版本，发布状态必须为 **Published**，版本标签也必须与 ZIP 内 `metadata.json` 的 `modVersion` 一致。发布资源的文件名必须严格为 `Endless_Trial.zip`。与已安装版本相同的版本不会触发更新。

试炼存档文件不包含在模组安装目录使用的 ZIP 中。请勿将存档文件放入更新 ZIP。重新安装游戏或模组前，建议另行备份重要存档数据。

## 故障排查

- **模组未显示：**检查上述目录结构，并确认存在 `metadata.json`、DLL 和 `endless_trial_floor` 文件。
- **未出现自动更新提示：**确认新版本标签高于已安装版本，发布状态不是 Draft 或 Prerelease，并检查 ZIP 文件名是否正确。
- **报告问题：**请提供游戏版本、模组版本、复现步骤，以及 `C:\Users\<用户名>\AppData\LocalLow\TEAMHORAY\Sephiria\Player.log` 中的相关内容。公开日志前，请检查其中是否包含个人信息。

## 许可与权利

本模组并非 TEAM HORAY 的官方产品。Sephiria 名称、原版游戏素材及音乐的权利归各自权利人所有。发布本模组并不意味着另行授予对这些原版素材的再使用许可。

本仓库目前未指定允许再使用模组代码的开源许可证。公开但未附带许可证的源代码，不应被视为允许自由修改或再发布。模组代码的开源许可证将在之后另行决定。
