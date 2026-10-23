# JMS Windows 桌面版

JMS（Jim608 Media Server）是基於 [DonutWare/Fladder](https://github.com/DonutWare/Fladder) 的 Jellyfin 用戶端。本倉庫專門提供 **Windows x64** 安裝程式、Portable ZIP 與 `update.json`。

## 畫面與功能

![JMS 功能總覽示意圖](https://raw.githubusercontent.com/jim608/JMS-Android/b7ed27260fa84e4ba0fc4e733ad7c89aafc0a6f3/docs/images/jms-overview.svg)

JMS 讓你在桌面瀏覽 Jellyfin 媒體庫、播放影片與選擇字幕，並透過原生介面使用自己的 Seerr 點片服務。

<table>
  <tr>
    <th width="65%">桌面深色字型預覽</th>
    <th width="35%">手機淺色字型預覽</th>
  </tr>
  <tr>
    <td align="center"><img src="https://raw.githubusercontent.com/jim608/JMS-Android/b7ed27260fa84e4ba0fc4e733ad7c89aafc0a6f3/docs/images/desktop-dark.png" alt="JMS 共用介面的合成字型預覽：桌面深色，非完整 App 截圖" width="640"></td>
    <td align="center"><img src="https://raw.githubusercontent.com/jim608/JMS-Android/b7ed27260fa84e4ba0fc4e733ad7c89aafc0a6f3/docs/images/mobile-light.png" alt="JMS 共用介面的合成字型預覽：手機淺色，非完整 App 截圖" width="280"></td>
  </tr>
</table>

**圖片說明：以上兩張為合成字型預覽，展示共用介面的文字層級，並非完整 App 截圖。** 手機圖僅用於呈現共用字型效果；本倉庫僅提供 Windows x64 發行檔。

![JMS 連線與使用流程示意圖](https://raw.githubusercontent.com/jim608/JMS-Android/b7ed27260fa84e4ba0fc4e733ad7c89aafc0a6f3/docs/images/jms-how-it-works.svg)

- **瀏覽媒體**：連線自己的 Jellyfin 伺服器，瀏覽媒體庫、搜尋作品並切換帳號。
- **播放與字幕**：選擇音軌與字幕；使用 MPV 播放時可用秒數輸入或滑軌微調字幕時間。雙軌及字幕格式能力依播放器與平台而定。
- **Seerr 點片**：使用自己設定的 Jellyseerr／Seerr 服務搜尋作品、查看申請紀錄及回報問題；登入與可用操作依服務權限決定。
- **環境光與睡眠**：提供可調強度、擴散範圍的播放環境光與睡眠計時，依觀看習慣安排播放。

## 下載與更新

目前公開測試版為 [JMS 0.11.1-jms.44+46](https://github.com/jim608/JMS-Desktop/releases/tag/v0.11.1-jms.44)，提供 Windows x64 [安裝程式](https://github.com/jim608/JMS-Desktop/releases/download/v0.11.1-jms.44/JMS-Windows-0.11.1-jms.44-x64-setup.exe)與 [Portable ZIP](https://github.com/jim608/JMS-Desktop/releases/download/v0.11.1-jms.44/JMS-Windows-0.11.1-jms.44-x64-portable.zip)。本版改善介面字體：繁體中文採用內建 Noto Sans TC，調整標題、內文與按鈕的字重及行距，提升閱讀舒適度。Discord 分享維持預設關閉，須另行同意。安裝程式及 App 均未簽章，使用前請閱讀版本說明中的驗證限制與更新注意事項。

公開版本以 [Releases](https://github.com/jim608/JMS-Desktop/releases) 為準，各版提供 Windows x64 安裝程式、Portable ZIP、更新資訊、SHA256 校驗清單、完整 App 來源及原生依賴材料。實機驗證限制與未簽章狀態詳見各版本說明。

自動檢查更新不會自動安裝；安裝前須由使用者確認，並核對平台、版本與 SHA256。穩定版不會接收測試版；未簽章版本可能顯示 Windows SmartScreen 提示，簽章狀態以各版本說明為準。

## 共用來源與其他平台

共用 Flutter 原始碼維護於 [JMS-Android 的 jms 分支](https://github.com/jim608/JMS-Android/tree/jms)，本倉庫不另存一份 lib/。每版附件提供精確 sourceCommit 對應的完整來源、校驗清單與原生依賴材料。GitHub 自動 Source code.zip 僅含發布倉庫文件；發布 tag 與共用來源提交分開記錄。

Linux（EndeavourOS／Arch x86_64）請使用 [JMS-Linux](https://github.com/jim608/JMS-Linux)。Windows 與 Linux 使用獨立發布庫，不互相作為更新備援。Android 使用 [JMS-Android](https://github.com/jim608/JMS-Android)。

## 授權

JMS 沿用 Fladder 的 GPLv3 授權，保留 DonutWare、原作者與第三方署名。原生材料依各平台實際散布的二進位檔核對；其他平台的驗證結果不代替 Windows 驗證。
