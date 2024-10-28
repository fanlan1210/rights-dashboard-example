## 學權儀表板：空白範本

本專案延伸自本人在擔任元智大學學生會資訊顧問期間，開發的[學權儀表板專案](rights.yzusa.tw)。

透過串接 Google 試算表方式，將學生會學權案件辦理情形，以統計儀表版的靜態網頁呈現。本網頁以 Vue 3 為基礎，搭配 tailwind CSS 進行樣式調整，圖表的部分使用 ECharts 繪製。

### 如何使用
以下將說明如何套用本專案至自身環境。

#### 建立資料表格（Google 試算表）

1. 首先請點選進入[學權儀表板範例](https://url.fanlan.net/rights-data)，可以看到範例試算表，請在這裡點選「檔案」->「建立副本」，將整份檔案另存至自身雲端
1. 此時便可以將首頁「專案進度」的內容進行編輯調整，符合自身需求
1. 調整完畢後，請將共用設定改為「知道連結的任何人都可檢視」，以便後續讓網頁擷取資料
1. 此時複製共用連結網址，將網址最後一段記錄下來，比如範本網址為 `https://docs.google.com/spreadsheets/d/1wUt8YqGlq8WcASUw69q-WgLHJ6BM1bxxxo2eMxtuXnY`，便要記錄 `1wUt8YqGlq8WcASUw69q-WgLHJ6BM1bxxxo2eMxtuXnY` 的部分，待會在網頁設定的部分會用到
1. 接著請點選進入「統計資料」分頁，在此時請查看瀏覽器網址列，會看到網址尾段會有一個 `gid=747570329` 的鍵值碼，也請將數字部分記錄下來，待會在網頁會用到

#### 網頁資料串接

1. 將前面複製下來的長字串，貼至 `index.html` 的第 94 行裡，此時將會把學權案件資料串接
2. 將前面複製下來的長字串，貼至 `index.html` 的第 145 行裡；將前面複製下來的數字部分，貼至 `index.html` 的第 146 行裡，此時將會把學權案件的統計資料串接
3. 可以編輯 `<head>` 內的各類標籤文字，讓網站更加完整具體

### 開發

[WIP]
*歡迎發 PR 更新說明！*
