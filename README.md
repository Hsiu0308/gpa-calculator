# GPA 計算機 (GPA Calculator Website)

這是一個互動式的 GPA (成績平均績點) 計算網站。使用者可以動態新增、刪除和排序課程，並即時獲得 GPA 計算結果。

## 🚀 即時網站預覽 (Live Demo)

您可以透過以下連結瀏覽這個網站的即時成果：

[**https://Hsiu0308.github.io/gpa-calculator/**](https://hsiu0308.github.io/gpa-calculator/)

---

## 專案結構

project/
├── index.html # 網站主頁
├── app.js # 核心 JavaScript 檔案
├── styles/ # 樣式檔案
│ ├── style.scss # SCSS 源碼
│ ├── style.css # 編譯後的 CSS
│ └── style.css.map # Source map 檔案
└── math.jpg # 載入動畫背景圖

## 💡 功能特色

- **即時 GPA 計算：** 根據使用者輸入的學分 (credits) 和成績 (grade)，即時計算加權平均 GPA。
- **動態表單操作：**
  - 使用者可以點擊「+」按鈕動態新增課程輸入欄位。
  - 使用者可以點擊「垃圾桶」圖示刪除任一筆課程資料，並觸發 `scaleDown` 動畫。
- **課程排序演算法：**
  - 可依據成績「升序」或「降序」排列所有課程。
  - 排序功能是使用 **Merge Sort (合併排序) 演算法** 實作，確保高效能。
- **GSAP 載入動畫：** 網頁開啟時，使用 GSAP (TimelineMax) 函式庫執行流暢的英雄 (Hero) 圖片與滑塊 (Slider) 動畫。
- **動態 UI 反饋：**
  - 根據選擇的成績 (A, B, C...)，下拉式選單會動態改變背景顏色 (例如 A 為綠色, F 為灰色)。
  - 最終 GPA 結果會顯示在一個有 `border_color` 動畫的圓形中。
- **課程自動完成：** 提供一個 `<datalist>` 包含大量課程選項，供使用者快速輸入。

## 🛠️ 使用技術

- HTML5
- CSS3 / SCSS
- JavaScript (ES6+)
- **GSAP (GreenSock Animation Platform):** 用於開場動畫。
- **Merge Sort Algorithm:** 用於課程排序邏輯。
- Font Awesome: 用於垃圾桶與新增圖示。
- Google Fonts (Baloo 2)

## 🔧 開發環境設置

1.  clone 此專案。
2.  安裝 SASS 編譯器 (如果尚未安裝)。
3.  執行 SASS watch 來自動編譯 SCSS 檔案 (請注意 `index.html` 中引用的路徑是 `styles/`):

```bash
sass --watch styles/style.scss styles/style.css
```

---

## 📝 作者

Hensel Huang

## 📄 授權

MIT License
