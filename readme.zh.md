# InsiderTweak

![Screenshot of InsiderTweak](https://i.imgur.com/YTtU1to.png)

**InsiderTweak Enroll** 是一款离线工具，可让您的 Windows 设备加入 Windows Insider 计划，无需 Microsoft 帐户或提交任何参与申请。非常适合注重隐私并希望跳过官方申请流程的用户。

- [English](readme.en.md)
- [简体中文](readme.zh.md)

---

## 主要功能

- **离线注册**  
  通过注册表直接切换到 Canary、Dev、Beta 或 Release Preview 渠道，无需在线批准。

- **快速更新检查**  
  一键菜单选项即可查询当前 Insider 渠道和系统版本号。

- **多语言界面**  
  支持英语、俄语和简体中文，可在脚本内即时切换。

- **隐私优先**  
  无需远程登录或开启额外的遥测，您的数据仅保存在本地。

---

## 要求

- Windows 11 或 Windows 10 版本 1809 及以上。  
- 管理员权限。

---

## 使用方法

1. 右键点击 **InsiderTweakEnroll.cmd** → **以管理员身份运行**。  
2. 选择通道、“检查更新”或“切换语言”。  
3. 如有提示，请重启以启用 Microsoft Flight Signing。  
4. 在 **设置 → 隐私和安全 → 诊断与反馈** 中确保诊断数据设置为 **完整**。

---

## 工作原理

脚本设置了未公开的注册表标志（例如 `TestFlags=0x20`），屏蔽了在线 Insider 服务的检查，并在本地应用所选配置。由于 Windows Update 不验证在线注册，只要注册表值正确，就能收到 Insider 预览版本。

---

## 恢复默认设置

选择“停止接收 Insider 版本”可删除所有 Insider 配置并禁用 Flight Signing。此操作需要重启系统。

---

## 许可证

MIT 许可证。详见 [LICENSE](LICENSE)。

---