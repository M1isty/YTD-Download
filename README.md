# YTD-Download
影片/音樂下載

影片、音樂與圖片下載器（YouTube、Instagram 貼文照片／Reels／限時動態、Threads、Facebook、Spotify 單曲／專輯／播放清單配對、一般檔案），以 yt-dlp 為下載核心。有 Windows 版與安卓版。

## 下載（分享給朋友用這兩個連結）
| 版本 | 下載連結 | 安裝方式 |
|---|---|---|
| Windows | https://github.com/M1isty/YTD-Download/releases/latest/download/YTD_Setup.bat | 雙擊下載的 `YTD_Setup.bat`，自動安裝並建立桌面捷徑 |
| 安卓 | https://github.com/M1isty/YTD-Download/releases/latest/download/YTD.apk | 在手機上點開 APK 安裝（需允許「安裝不明來源的應用程式」） |
| 安卓（32 位元舊手機） | https://github.com/M1isty/YTD-Download/releases/latest/download/YTD_32bit.apk | 一般版安裝時顯示「套件似乎無效」才用這個 |

Windows 第一次執行 `.bat` 可能出現「Windows 已保護您的電腦」，按「其他資訊 → 仍要執行」即可。

## 更新
- **程式本身**：Windows 版點上方版本號 →「檢查更新」；安卓版到下方「更新」分頁。程式會讀取本儲存庫的 `updates/latest.json`（Windows）與 `updates/android.json`（安卓）。
- **下載核心 yt-dlp**：網站改版造成無法下載時，Windows 版按「更新下載核心」、安卓版在「更新」分頁按「更新下載核心」，可選穩定版或每日更新版。

本儲存庫必須是**公開**的，朋友才能下載與線上更新（不需要任何金鑰）。若改回私人，只有在程式設定裡填了唯讀金鑰的人才能更新。

## 目錄
| 路徑 | 內容 |
|---|---|
| `updates/` | 線上更新用：`latest.json`、最新更新包 `YTD_Vx.x.xx.zip`、`android.json` |
| `installer/YTD_Setup.bat` | Windows 安裝檔（固定檔名，也會上傳到 Release） |

原始碼不在本儲存庫公開。

## 發佈新版本
每次發佈時，`YTD_Setup.bat`、`YTD.apk`、`YTD_32bit.apk` 要放在**同一個、最新的** Release 裡，下載連結才會正確。
安卓版的簽章存在建置電腦的 `%LOCALAPPDATA%\YTD-Android\keystore`，請備份；換了簽章，舊版 App 就無法直接覆蓋更新。
