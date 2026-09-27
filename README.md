# JMS Desktop

JMS（Jim608 Media Server）是基於 Fladder 的 Jellyfin 用戶端。本儲存庫提供 Windows 與 Linux 桌面版的發布渠道；所有平台共用同一份 Flutter 原始碼。

## 下載狀態

目前尚無可公開下載的桌面版 Release。Windows 原生依賴的來源材料正在核對；EndeavourOS 安裝包正在建置與驗證。儲存庫存在不代表安裝包或線上升級已可使用。

完成檢查後，安裝檔會放在 [Releases](https://github.com/jim608/JMS-Desktop/releases)，不放進一般程式碼歷史。

## 平台與更新

- **Windows x64**：安裝程式、Portable ZIP，以及 App 內檢查、下載及確認安裝更新。
- **EndeavourOS／Arch Linux x64**：pacman 套件與可攜式壓縮包。使用系統 MPV、GTK 3 與 ALSA；安裝更新需由使用者確認並取得系統授權。
- Windows 與 Linux 共用本儲存庫的 Release，分別使用 `update.json` 與 `update-linux.json`，不混用平台安裝檔。
- 自動檢查不等於自動安裝。首次安裝需手動完成；測試版須啟用「接收測試版」。沒有公開版本時，App 不會憑空取得更新。
- **Web** 使用 [JMS-Web](https://github.com/jim608/JMS-Web) 部署，不提供 App 自動更新。

## 共用來源

[唯一 Flutter 來源](https://github.com/jim608/JMS-Android/tree/jms)維護共用介面、登入、點片及播放器整合。本儲存庫不另維護一份 `lib/`。每次發布均須附上對應來源提交、建置識別與檔案校驗資訊。

## 授權與注意事項

JMS 沿用 Fladder 的 GPL-3.0 授權，保留原作者 DonutWare 及其他貢獻者署名。對應來源與第三方材料依平台發布；未簽章 Windows 測試版可能觸發 SmartScreen。EndeavourOS 的 GPU 播放、登入及覆蓋安裝仍需實機驗證。
