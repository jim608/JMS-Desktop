# JMS Windows 桌面版

JMS（Jim608 Media Server）是基於 [DonutWare/Fladder](https://github.com/DonutWare/Fladder) 的 Jellyfin 用戶端。本倉庫專門提供 **Windows x64** 安裝程式、Portable ZIP 與 `update.json`。

## 下載與更新

正式可下載版本以 [Releases](https://github.com/jim608/JMS-Desktop/releases) 為準。Windows 原生依賴與來源材料依實際資產逐項核對，完成發布條件前不提供未核對的更新入口。

自動檢查更新不會自動安裝；安裝前須由使用者確認，並核對平台、版本與 SHA256。穩定版不會接收測試版；未簽章版本可能顯示 Windows SmartScreen 提示，簽章狀態以各版本說明為準。

## 共用來源與其他平台

共用 Flutter 原始碼維護於 [JMS-Android 的 jms 分支](https://github.com/jim608/JMS-Android/tree/jms)，本倉庫不另存一份 lib/。每版附件提供精確 sourceCommit 對應的完整來源、校驗清單與原生依賴材料。GitHub 自動 Source code.zip 僅含發布倉庫文件；發布 tag 與共用來源提交分開記錄。

Linux（EndeavourOS／Arch x86_64）請使用 [JMS-Linux](https://github.com/jim608/JMS-Linux)。Windows 與 Linux 使用獨立發布庫，不互相作為更新備援。Android 使用 [JMS-Android](https://github.com/jim608/JMS-Android)，Web 使用 [JMS-Web](https://github.com/jim608/JMS-Web)。

## 授權

JMS 沿用 Fladder 的 GPLv3 授權，保留 DonutWare、原作者與第三方署名。原生材料依各平台實際散布的二進位檔核對；其他平台的驗證結果不代替 Windows 驗證。
