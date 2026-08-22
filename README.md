# DSH Mobile

DSH 手机端：DeepSeek Harness Desktop 的安卓远程客户端（WebView 壳）。

- 扫码配对桌面面板二维码，手机远程控制 DSH
- 地址簿、全屏模式、自动更新
- DeepSeek 余额查询（App 菜单 → DeepSeek 信息）

## 自动更新

`version.json` 为更新清单，App 启动时检查。发布新版：

```powershell
.\publish-update.ps1 -VersionName 1.4 -Repo zwmhua2-lab2/dsh-mobile
```

或手动：构建 APK → 更新 `version.json`（versionCode/versionName/apkUrl）→ 上传 APK 到 GitHub Release → 提交 `version.json`。
