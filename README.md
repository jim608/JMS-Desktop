# JMS Windows 桌面版

JMS（Jim608 Media Server）是基於 [DonutWare/Fladder](https://github.com/DonutWare/Fladder) 的 Jellyfin 用戶端。本倉庫專門提供 **Windows x64** 安裝程式、Portable ZIP 與 `update.json`。

## 畫面與功能

JMS 讓你瀏覽自己的 Jellyfin 媒體庫、播放影片與選擇字幕，並透過原生介面使用自己的 Seerr 點片服務。

以下為 **JMS `.44` Web 完整 App 的實際執行截圖**，使用本機示範資料及原創封面，沒有重繪介面。桌面／手機寬度展示共用 UI，不是本倉庫原生平台或手機硬體的驗收證據。

<table>
  <tr><th>桌面首頁</th><th>手機寬度首頁</th></tr>
  <tr>
    <td width="72%"><img src="https://raw.githubusercontent.com/jim608/JMS-Android/5a26ee3e80b05a6b49b13e3f34baf8c650b294fd/docs/images/jms-desktop-home.png" alt="JMS .44 Web 實際桌面首頁，本機示範資料" width="100%"></td>
    <td width="28%"><img src="https://raw.githubusercontent.com/jim608/JMS-Android/5a26ee3e80b05a6b49b13e3f34baf8c650b294fd/docs/images/jms-mobile-home.png" alt="JMS .44 Web 實際手機寬度首頁，本機示範資料" width="100%"></td>
  </tr>
  <tr><th>桌面影片詳細頁</th><th>手機寬度影片詳細頁</th></tr>
  <tr>
    <td><img src="https://raw.githubusercontent.com/jim608/JMS-Android/5a26ee3e80b05a6b49b13e3f34baf8c650b294fd/docs/images/jms-desktop-details.png" alt="JMS .44 Web 實際影片詳細頁" width="100%"></td>
    <td><img src="https://raw.githubusercontent.com/jim608/JMS-Android/5a26ee3e80b05a6b49b13e3f34baf8c650b294fd/docs/images/jms-mobile-details.png" alt="JMS .44 Web 實際手機寬度影片詳細頁" width="100%"></td>
  </tr>
</table>

**Discord 實際播放卡片**：使用者提供並同意公開作品名稱、封面及進度。此圖代表當次顯示結果，封面整合仍在驗證。

![Discord 實際顯示 JMS 播放狀態](https://raw.githubusercontent.com/jim608/JMS-Android/5a26ee3e80b05a6b49b13e3f34baf8c650b294fd/docs/images/discord-presence.png)

[圖片來源與標示](https://github.com/jim608/JMS-Android/blob/5a26ee3e80b05a6b49b13e3f34baf8c650b294fd/docs/images/README.md)

- **瀏覽媒體**：連線自己的 Jellyfin 伺服器，瀏覽媒體庫、搜尋作品並切換帳號。
- **播放與字幕**：選擇音軌與字幕；使用 MPV 播放時可用秒數輸入或滑軌微調字幕時間。雙軌及字幕格式能力依播放器與平台而定。
- **Seerr 點片**：使用自己設定的 Jellyseerr／Seerr 服務搜尋作品、查看申請紀錄及回報問題；登入與可用操作依服務權限決定。
- **環境光與睡眠**：提供可調強度、擴散範圍的播放環境光與睡眠計時，依觀看習慣安排播放。

## 下載與更新

目前公開測試版為 [JMS 0.11.1-jms.45+47](https://github.com/jim608/JMS-Desktop/releases/tag/v0.11.1-jms.45)，提供 Windows x64 [安裝程式](https://github.com/jim608/JMS-Desktop/releases/download/v0.11.1-jms.45/JMS-Windows-0.11.1-jms.45-x64-setup.exe)與 [Portable ZIP](https://github.com/jim608/JMS-Desktop/releases/download/v0.11.1-jms.45/JMS-Windows-0.11.1-jms.45-x64-portable.zip)。本版新增「一起看」：朋友各自登入同一台 Jellyfin，在播放器建立房間或輸入 6 位房間碼加入，同步播放、暫停及跳轉。Discord 分享維持預設關閉，須另行同意。安裝程式及 App 均未簽章，使用前請閱讀版本說明中的驗證限制與更新注意事項。

公開版本以 [Releases](https://github.com/jim608/JMS-Desktop/releases) 為準，各版提供 Windows x64 安裝程式、Portable ZIP、更新資訊、SHA256 校驗清單、完整 App 來源及原生依賴材料。實機驗證限制與未簽章狀態詳見各版本說明。

自動檢查更新不會自動安裝；安裝前須由使用者確認，並核對平台、版本與 SHA256。穩定版不會接收測試版；未簽章版本可能顯示 Windows SmartScreen 提示，簽章狀態以各版本說明為準。

## 共用來源與其他平台

共用 Flutter 原始碼維護於 [JMS-Android 的 jms 分支](https://github.com/jim608/JMS-Android/tree/jms)，本倉庫不另存一份 lib/。每版附件提供精確 sourceCommit 對應的完整來源、校驗清單與原生依賴材料。GitHub 自動 Source code.zip 僅含發布倉庫文件；發布 tag 與共用來源提交分開記錄。

Linux（EndeavourOS／Arch x86_64）請使用 [JMS-Linux](https://github.com/jim608/JMS-Linux)。Windows 與 Linux 使用獨立發布庫，不互相作為更新備援。Android 使用 [JMS-Android](https://github.com/jim608/JMS-Android)。

## 授權

JMS 沿用 Fladder 的 GPLv3 授權，保留 DonutWare、原作者與第三方署名。原生材料依各平台實際散布的二進位檔核對；其他平台的驗證結果不代替 Windows 驗證。
