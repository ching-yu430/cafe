# 嘉義老屋咖啡廳探訪記

> *用一張老派記錄卡，留住每間老屋咖啡廳的靈魂。*

**Chiayi Old-House Café Journal** — 一個為慢旅行者設計的靜態網頁工具，以昭和文件美學記錄嘉義老屋咖啡廳的探訪體驗。

---

## ✦ 專案簡介

嘉義擁有全台密度最高的日治時期老屋群，近年逐漸被轉化為獨立咖啡廳與選物店。這個工具幫助你在造訪後留下一張完整的「探訪記錄卡」，包含甜點、空間靈魂、停車資訊、消費價位，以及最重要的——那些只有親身感受才能描述的細節。

所有資料儲存於瀏覽器本地端（`localStorage`），不上傳任何伺服器，完全離線可用。

---

## ✦ 功能一覽

| 功能 | 說明 |
|------|------|
| 📝 探訪表單 | 8 個欄位，完整記錄每間老屋咖啡廳的核心資訊 |
| ★ 星等評分 | 1–5 顆星，附文字說明標籤 |
| 🅿 停車友善性 | 五段式選擇，從「很難停」到「專屬車位」 |
| ¥ 消費價位 | 四段制（平價 ¥ 至高價 ¥¥¥¥） |
| 🔄 回訪意願 | 0–100 滑桿，附區間文字描述 |
| # 自動標籤 | 依甜點關鍵字（布丁、可頌、塔…）自動生成 Hashtag |
| 📋 複製功能 | 一鍵複製純文字版記錄卡，可直接貼到筆記或社群 |
| 🗂 探訪側欄 | 歷史記錄側邊欄，隨時切換查閱過去的造訪 |
| 🖨 列印輸出 | 支援瀏覽器列印，可存為 PDF |

---

## ✦ 快速開始

本專案為**純靜態單頁應用**，無需安裝任何依賴。

```bash
# 1. Clone 此專案
git clone https://github.com/your-username/chiayi-cafe-journal.git

# 2. 直接用瀏覽器開啟
open index.html
```

或直接部署至 GitHub Pages：

```
Settings → Pages → Deploy from branch → main / (root)
```

---

## ✦ 專案結構

```
chiayi-cafe-journal/
├── index.html               # 主程式（單一 HTML 檔，含 CSS + JS）
├── assets/
│   └── example_prompt.txt   # 三筆完整範例資料與填寫說明
└── references/
    └── data_sources.txt     # 嘉義老屋資料來源、設計靈感、字型授權
```

---

## ✦ 技術細節

- **框架**：無（Vanilla HTML / CSS / JavaScript）
- **字型**：Noto Serif TC + Shippori Mincho（Google Fonts CDN）
- **資料儲存**：`localStorage`，鍵值為 `chiayi_cafe_journal`
- **背景紙紋**：內嵌 SVG `feTurbulence` 濾鏡，無外部圖片依賴
- **色系**：昭和建材色調（cream / parchment / coffee / espresso / sage）

---

## ✦ 截圖

> 昭和文件美學的表單設計，兼顧資訊密度與閱讀質感。

*（可在此插入 screenshot.png）*

---

## ✦ 自動標籤對照表

填入「招牌甜點」欄位時，以下關鍵字會自動生成對應 Hashtag：

| 輸入關鍵字 | 自動生成標籤 |
|-----------|-------------|
| 布丁 | `#焦糖布丁` `#布丁控` |
| 戚風 | `#戚風蛋糕` `#雲朵口感` |
| 可頌 | `#可頌控` `#奶油香` |
| 磅蛋糕 | `#磅蛋糕` `#英式下午茶` |
| 起司 | `#起司蛋糕` `#乳酪控` |
| 塔 | `#甜塔` `#法式甜點` |
| 瑪德蓮 | `#瑪德蓮` `#法式小點` |
| 司康 | `#司康` `#英式下午茶` |

所有記錄自動附加 `#嘉義老屋` `#老屋咖啡廳` 基礎標籤。

---

## ✦ 授權

本專案以 **MIT License** 開放授權，歡迎自由 fork 改作。

字型依各自 SIL Open Font License 1.1 授權使用。

---

## ✦ 貢獻方式

若你有造訪嘉義老屋咖啡廳的記錄、想新增的功能，或發現 Bug，歡迎開 Issue 或送 Pull Request。

尤其歡迎：
- 補充 `references/data_sources.txt` 的田野調查筆記
- 新增自動標籤關鍵字
- 分享你的探訪截圖至 Discussions

---

<p align="center">
  嘉義老屋咖啡廳探訪記 &nbsp;·&nbsp; Chiayi Café Journal<br>
  <sub>為每一間值得被記住的老屋，留下一張記錄卡。</sub>
</p>
