<div align="center">
	<img width="80" height="80" src="https://cdn.jsdelivr.net/gh/Tomotoes/images/blog/icon.png" alt="tomoto">
	<br>
	<h1>Scrcpy GUI</h1>
	<sub>Built with ❤︎ by <a href="https://tomotoes.com">Simon Ma</a> - <a href="https://github.com/Hs0/scrcpy-gui">English document</a><br>Translated by XXXF</sub>
</div>
<hr/>
<p align="center">✨ <strong>一個簡潔&漂亮的 scrcpy GUI 應用</strong></p>
<p align="center">
  <a href="https://github.com/feross/standard">
    <img src="https://img.shields.io/badge/code%20style-standard-green.svg?style=flat-square" alt="">
  </a>
  <a href="https://github.com/Tomotoes/scrcpy-gui/releases">
    <img src="https://img.shields.io/github/downloads/Tomotoes/scrcpy-gui/total.svg?style=flat-square" alt="">
  </a>
   <a href="https://travis-ci.org/Tomotoes/scrcpy-gui/builds">
    <img src="https://img.shields.io/travis/Tomotoes/scrcpy-gui.svg?style=flat-square" alt="">
  </a>
  <a href="https://github.com/Tomotoes/scrcpy-gui/releases/latest">
    <img src="https://img.shields.io/github/release/Tomotoes/scrcpy-gui.svg?style=flat-square" alt="">
  </a>
  <a href="https://gitter.im/scrcpy/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge"><img src="https://badges.gitter.im/scrcpy/community.svg?style=flat-square"></a>
  <a href="https://opensource.org/licenses/GPL-3.0/"><img src="https://badges.frapsoft.com/os/gpl/gpl.svg?style=flat-square"></a>
  <a href="https://github.com/Tomotoes/scrcpy-gui/issues"><img src="https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat-square"></a>
</p>



## 💡簡介

<p align="center"><a href="https://jq.qq.com/?_wv=1027&k=5jxRe2o" target="_blank">點擊連結加入原作者的QQ群聊【Scrcpy-GUI】</a></p><p align="center"><a href="https://mp.weixin.qq.com/s/JbD05YUlQ7NvSCsPJTm5nQ" target="_blank"><strong>Topbook:</strong> 不用花錢，三步投射裝置到任何電腦系統，支持高幀率螢幕錄影、電腦控制裝置。</a></p>
<p align="right"> 感謝 Topbook 平台的分享!</p>
<div align=center><img width="508" height="785.6" src="https://cdn.jsdelivr.net/gh/Tomotoes/images/scrcpy-gui/Chinese.gif"/></div>
<div align=center><img src="./screenshot.gif"/></div>

[Scrcpy](https://github.com/Genymobile/scrcpy) 是由流行的`Android`模擬器`Genymotion`背後的團隊創建的，但它本身並不是`Android`模擬器，它顯示和控制透過`USB`（或透過`TCP/IP`）連接的`Android`裝置，它不需要任何`root`訪問權限，它適用於`GNU/Linux`、`Windows`和`MacOS`。

`Scrcpy`的運作原理是在你的`Android`裝置上啟動伺服器，桌面應用程式使用`USB`（或使用`ADB`隧道無線）進行通訊。伺服器器流式傳輸裝置螢幕的[H.264](https://translate.googleusercontent.com/translate_c?depth=1&rurl=translate.google.com&sl=en&sp=nmt4&tl=zh-CN&u=https://en.wikipedia.org/wiki/H.264/MPEG-4_AVC&xid=25657,15700019,15700124,15700186,15700190,15700201,15700237,15700242,15700248&usg=ALkJrhiJZJWaUqBVRqUviQ4IlhKQCwqp_Q)視訊。 客户端解碼視訊幀並顯示它們。客户端捕獲輸入（鍵盤和滑鼠）事件，將它們發送到伺服器，伺服器將它們注入裝置。[文件](https://github.com/Genymobile/scrcpy/blob/master/DEVELOP.md)提供了更多詳細資訊。

如果你想在桌面上看到你的`Android`螢幕與應用程式或内容進行交互，記錄你的裝置螢幕或執行其他基本任務，那`Scrcpy`就是一個好的選擇。

簡而言之，`Scrcpy`是一種很好的方式，可以在你的電腦上輕鬆查看你的`Android`螢幕畫面，並且可以即時與其進行交互操作。

*引用自[云网牛站](https://ywnz.com/linuxsj/5581.html)*



## ✨特色

- **輕量化** （原版，僅顯示裝置螢幕畫面）
- **高效能** （30~60fps）
- **高解析度** （1920×1080或以上）
- **低延遲** （70~100ms）
- **啟動時間短** （顯示第一章圖像約1秒）
- **非侵入性** （裝置上沒有安裝任何東西）
- **不需要 ROOT**
- **有線無線都可連接**
- **可以隨意調整界面和碼率**
- **畫面随意裁切，自帶螢幕錄影（手游直播利器）**
- **支援多裝置同時投影螢幕**
- **利用電腦的鍵盤和滑鼠可以控制裝置**
- **把 APK 文件拖拽到電腦視窗即可安裝應用程式到裝置，把普通檔案拖拽到視窗即可複製到裝置**
- **裝置電腦共用剪貼簿**
- **自動檢測USB連接的裝置**
- **可直接添加裝置的區域連線IP，達到無線控制的效果**
- **將自動保存連接過的IP地址，下次輸入時，自動提醒**
- **支持裝置别名**
- **支持中英兩種语言，另外增加繁體中文翻譯**
- **Tray menu**
- 等等等...

*部分引用自[最美應用](http://zuimeia.com/app/6771/?platform=2)*



## 🌞要求

1. `Android 5.0`以上

2. 開啟USB偵錯

   在 `開發人員選項` 開啟 `USB偵錯`，USB連接裝置
   ![img](https://cdn.jsdelivr.net/gh/Tomotoes/images/scrcpy-gui/1.jpg)

3. 安裝好`ADB` ，並配置環境變數。

   [Windows](https://dl.google.com/android/repository/platform-tools-latest-windows.zip)
   [Mac OS](https://dl.google.com/android/repository/platform-tools-latest-darwin.zip)
   [Linux](https://dl.google.com/android/repository/platform-tools-latest-linux.zip)

   在任何路徑下開啟命令提示字元(CMD)，輸入 `ADB` 有回應。

4. 安装好`scrcpy`，並配置環境變數

  - Windows

    Windows 可以使用包含所有依賴項目（包括adb）的預先建構存檔：

    下載下面`scrcpy`的壓縮檔，裡面有`ADB`檔案，然後把解壓縮後的`scrcpy`資料夾添加到環境變數，再將電腦重新開機，就可以了。

    1. [`scrcpy-win32-v1.10.zip`](https://github.com/Genymobile/scrcpy/releases/download/v1.10/scrcpy-win32-v1.10.zip)
       *(SHA-256: f98b400b3764404b33b212e9762dd6f1593ddb766c1480fc2609c94768e4a8e1)*
    2. [`scrcpy-win64-v1.10.zip`](https://github.com/Genymobile/scrcpy/releases/download/v1.10/scrcpy-win64-v1.10.zip)
       *(SHA-256: 95de34575d873c7e95dfcfb5e74d0f6af4f70b2a5bc6fde0f48d1a05480e3a44)*

    你也可以[手動編譯](https://github.com/Genymobile/scrcpy/blob/master/BUILD.md)。

  - Mac OS

    可以使用 [Homebrew](https://brew.sh/) 來安裝：

    ```
    brew install scrcpy
    ```

    如果你還沒有安裝`ADB`，可以使用下面的指令：

    ```
    brew cask install android-platform-tools
    ```

    你也可以[手動編譯](https://github.com/Genymobile/scrcpy/blob/master/BUILD.md)。

  - Linux

    你可能需要[手動編譯應用程式](https://github.com/Genymobile/scrcpy/blob/master/BUILD.md)。別擔心，這並不難。

    此外，提供了 [Snap](https://en.wikipedia.org/wiki/Snappy_(package_manager)) 包：[`scrcpy`](https://snapstats.org/snaps/scrcpy)

    對於 Arch Linux， 可以使用 [AUR](https://wiki.archlinux.org/index.php/Arch_User_Repository) 包：[`scrcpy`](https://aur.archlinux.org/packages/scrcpy/)

    對於 Gentoo，可以使用 [Ebuild](https://wiki.gentoo.org/wiki/Ebuild) 包： [`scrcpy/`](https://github.com/maggu2810/maggu2810-overlay/tree/master/app-mobilephone/scrcpy)



## 🎉安裝

點擊此處下載[應用](https://github.com/Hs0/scrcpy-gui/releases)。



## 🎇使用

### 連接方式

#### 必須條件

- 請確保 **adb , scrcpy** 可正常使用
- 請確保裝置已開啟 USB 偵錯, 並已授權電腦偵錯

#### 有線连接

1. 請確保裝置已透過數據線連接到電腦

2. 等待程式自動偵測到裝置
3. 選中裝置，點擊`開啟選中的投影`
4. 等待裝置開啟

#### 無線連接

1. 請確保裝置與電腦處於同一區域連線

2. 第一次無線連接時:
   - **請確保裝置已透過數據線連接到電腦**
   - **請確保只有一台裝置經由數據線連接到電腦**
   - 第一次需設置端口，以後連接裝置，只需要添加裝置的固定IP即可

3. 輸入裝置的區域連線`IP`地址（如果`IP`為`DHCP`指派，請更改為固定`IP`）

4. 點擊`開啟無線連接`

5. 等待無線連接成功

6. 選中裝置，點擊`開啟選中的投影`

7. 等待裝置開啟



### 快速鍵

| 操作                             | 快速鍵                       | 快速鍵 (macOS)              |
| -------------------------------- | ---------------------------- | --------------------------- |
| 切換全螢幕模式                    | `Ctrl`+`f`                   | `Cmd`+`f`                   |
| 將視窗调整為 1:1                 | `Ctrl`+`g`                   | `Cmd`+`g`                   |
| 調整視窗大小以删除黑色邊框       | `Ctrl`+`x` \| *雙擊黑色背景* | `Cmd`+`x` \| *雙擊黑色背景* |
| 裝置`HOME`鍵                     | `Ctrl`+`h` \| *滑鼠中鍵*     | `Ctrl`+`h` \| *滑鼠中鍵*    |
| 裝置`BACK`鍵                     | `Ctrl`+`b` \| *滑鼠右鍵*     | `Cmd`+`b` \| *滑鼠右鍵*     |
| 裝置`多工切換`鍵                 | `Ctrl`+`s`                   | `Cmd`+`s`                   |
| 裝置`選單`鍵                     | `Ctrl`+`m`                   | `Ctrl`+`m`                  |
| 裝置`音量+`鍵                    | `Ctrl`+`↑`                   | `Cmd`+`↑`                   |
| 裝置`音量-`鍵                    | `Ctrl`+`↓`                   | `Cmd`+`↓`                   |
| 裝置`電源`鍵                     | `Ctrl`+`p`                   | `Cmd`+`p`                   |
| 喚醒裝置螢幕                     | *滑鼠右鍵*                   | *滑鼠右鍵*                  |
| 關閉裝置螢幕（保持投影）         | `Ctrl`+`o`                   | `Cmd`+`o`                   |
| 展开通知面板                     | `Ctrl`+`n`                   | `Cmd`+`n`                   |
| 折叠通知面板                     | `Ctrl`+`Shift`+`n`           | `Cmd`+`Shift`+`n`           |
| 將裝置剪貼簿中的内容複製到電腦　 | `Ctrl`+`c`                   | `Cmd`+`c`                   |
| 將電腦剪貼簿中的内容貼上到裝置 　| `Ctrl`+`v`                   | `Cmd`+`v`                   |
| 將電腦剪貼簿中的内容複製到裝置 　| `Ctrl`+`Shift`+`v`           | `Cmd`+`Shift`+`v`           |
| 安裝`APK`                        | 將`APK`檔案拖入投影          | 將`APK`檔案拖入投影         |
| 傳輸檔案到裝置                   | 將檔案拖入投屏               | 將檔案拖入投影              |
| 啟用/禁用FPS計數器（stdout）     | `Ctrl`+`i`                   | `Cmd`+`i`                   |



## 🎯開發

This project was generated with [electron-vue](https://github.com/SimulatedGREG/electron-vue)@[8fae476](https://github.com/SimulatedGREG/electron-vue/tree/8fae4763e9d225d3691b627e83b9e09b56f6c935) using [vue-cli](https://github.com/vuejs/vue-cli). Documentation about the original structure can be found [here](https://simulatedgreg.gitbooks.io/electron-vue/content/index.html).

如果你有任何問題，歡迎提交 `Issues` 或 `PR`！

``` bash
# install dependencies
npm install

# serve with hot reload at localhost:9080
npm run dev

# build electron application for production
npm run build

# lint all JS/Vue component files in `src/`
npm run lint
```



## 🤞貢獻者

<table>
  <tr>
    <td align="center"><a href="https://github.com/Tomotoes"><img src="https://avatars1.githubusercontent.com/u/32236122?s=460&v=4" width="100px;" alt="Tomotoes"/><br /><sub><b>Simon Ma</b></sub></a><br /><a href="https://github.com/Tomotoes/scrcpy-gui/commits?author=Tomotoes" title="Code">💻</a> <a href="https://tomotoes.com">🎨</a></td>
    <td align="center"><a href="https://github.com/Hs0"><img src="https://avatars2.githubusercontent.com/u/14960173?s=460&v=4" width="100px;" alt="XXXF"/><br /><sub><b>XXXF</b></sub></a><br />繁體中文化翻譯</td>
  </tr>  
</table>



## 👀贊助

如果你喜歡`scrcpy-gui`，並且它對你確實有幫助，歡迎給原作者贊助一杯咖啡~

paypal: [https://paypal.me/tomotoes](https://paypal.me/tomotoes)

支付寶：

![alipay](https://cdn.jsdelivr.net/gh/Tomotoes/images/blog/alipay.png)

微信：

![wechat](https://cdn.jsdelivr.net/gh/Tomotoes/images/blog/wechat.png)

## 📃協議

**GNU GPLv3**
