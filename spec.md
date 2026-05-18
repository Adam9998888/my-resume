# Resume Portfolio Website Spec

## 1. 目標
建立一個單頁式履歷型 portfolio 網站，符合 Apple Liquid Glass 風格，可直接部署到 GitHub Pages。網站內容以「學生履歷資料」為範例，未來可替換為真實個人資訊。

## 2. 核心需求
- 單一 `index.html` 檔案
- CSS 內嵌在 `<style>` 區塊，不使用外部樣式表
- 不使用 React / Vue / 任何打包工具
- 手機與桌面版皆適配，具備響應式佈局
- 用 Apple Liquid Glass 視覺語彙設計
- 包含 8 大區塊，且依序排列
- 頁面頂部需有浮動 TOC 導覽列，支援 smooth scroll

## 3. 視覺風格
### Apple Liquid Glass
- 背景採用深藍到紫粉漸層光暈，具柔和光澤感
- 卡片使用半透明白底，帶 `backdrop-filter: blur(24px)` 或類似模糊效果
- 卡片邊框為 1px 半透明白色，並搭配細緻陰影與 glow hover
- 元素圓角柔和，膠囊狀按鈕與標籤
- 文字保持高對比與可讀性，避免因玻璃效果導致閱讀困難

## 4. 響應式規格
- 手機：單欄垂直排列，內容寬度適應螢幕，TOC 可橫向滾動
- 平板/桌面：內容區塊具卡片分區、適度分欄，Timeline 與卡片 Grid 顯示良好
- 主要斷點：480px、768px、1024px

## 5. 首頁區塊架構
### 1. Hero
- 左側 / 上方：頭像（圓形）、名字、定位一句話
- 求職方向 pills：例如「AI 工程師」、「FinTech」、「科技業」
- 以視覺區隔 Hero 與其餘內容

### 2. About 關於我
- 2-3 段自我介紹文字
- 關鍵資訊摘要：求職方向、所在地、語言
- 內容呈現方式簡潔、易讀

### 3. Skills 核心技能
- 分類成多組技能標籤雲
- 每組採膠囊標籤形式，背景半透、邊框對比
- 最少 4-5 類別，示範資料可包含程式、AI 協作工具、專案管理、語言、軟實力

### 4. Education 學歷
- Timeline 樣式
- 每筆學歷包含學校、學系、年分、簡要描述
- 左側或右側顯示垂直軸、圓點、發光效果

### 5. Experience 經歷
- Timeline 樣式，含量化成果重點
- 每筆工作/專案有職稱、時間、公司/單位、數字化成果條列
- 使用發光圓點與軸線區分節點

### 6. Awards 競賽獎項
- 卡片 Grid 佈局
- 每張卡片含獎項名稱、年份、簡要描述、Emoji badge
- Grid 在桌面為 2-3 欄，手機單欄顯示

### 7. Projects 作品集
- 卡片 Grid 佈局
- 每張卡片含作品名稱、類型、簡述、可能的技術標籤
- 卡片具 hover 浮動效果

### 8. Contact 聯絡
- 4 顆按鈕：Email、GitHub、LinkedIn、IG
- 每顆按鈕採膠囊樣式，具玻璃感與 icon 提示
- 置底呼應整體主題

## 6. 頂部浮動 TOC
- sticky position fixed / sticky 於頁面頂端
- 包含 7 個錨點：關於 / 技能 / 學歷 / 經歷 / 獎項 / 作品 / 聯絡
- 手機版 TOC 可橫向滾動，避免按鈕擠在一起
- 點擊後平滑捲動至對應區塊

## 7. 互動細節
- smooth scroll for anchor links
- 卡片 hover 提升光暈與微浮動
- TOC active state 可選擇性加臨時樣式

## 8. 交付物
- `my-resume/index.html`
- 內含整體 HTML 與 `<style>` CSS
- 內容示範使用學生假資料（王小明 / 中原大學資管系)

## 9. GitHub Pages
- 由你自行 push 至 GitHub Pages 時，單一 `index.html` 即可部署
- 若需要，後續可提供「部署步驟說明」

## 10. 確認事項
請確認以下內容是否符合預期：
1. 是否同意以 Apple Liquid Glass 風格為整體視覺方向？
2. 是否同意使用單一 `index.html` + 內嵌 `<style>` 的方案？
3. 是否要我先依此 spec 進行原始頁面開發？
4. 是否希望我先輸出假資料版的完整 HTML，再讓你替換成真實資訊？

---

`spec.md` 已依你的要求建立，待你確認後再開始開發。