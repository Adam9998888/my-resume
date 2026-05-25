# Resume Portfolio Website Spec

## 1. 目標
建立一個單頁式履歷型 portfolio 網站，符合 Apple Liquid Glass 風格，可直接部署到 GitHub Pages。網站內容以「學生履歷資料」為範例，未來可替換為真實個人資訊。

## 2. 核心要求
- 單一 `index.html`，CSS 僅限於 `<style>` 區塊
- 不使用 React / Vue / 任何打包工具
- 手機與桌面皆適配，支援響應式佈局
- 只改 `index.html` 內的 `<style>`，不重寫 html 結構
- 頁面整體以 Apple Liquid Glass 視覺為核心
- 先確認此 `spec.md`，再開始開發

## 3. Apple Liquid Glass 視覺規格
- 背景使用兩個 radial-gradient 漸層光暈，從深藍延伸到紫粉，帶出輕柔光暈感
- 背景要有緩慢飄動效果，以 subtle animation 呈現
- 卡片為半透明白底，使用 `backdrop-filter: blur(24px)` 且兼容 `-webkit-backdrop-filter`
- 卡片邊框 1px 半透明白色
- hover 時卡片應展現柔光浮起效果，包含微量上移、柔和 glow、邊框變亮
- Timeline 需有左側垂直軸與圓點節點，圓點帶發光效果
- Tag 雲採膠囊狀、半透明背景、對比邊框
- 文字需保持高對比與清晰可讀
- UI 元素圓角柔和，符合 macOS Big Sur / iOS Control Center 玻璃質感

## 4. 響應式規格
- 手機：單欄排列，TOC 橫向滾動
- 平板/桌面：多欄佈局、Grid 內容適度延伸
- 主要斷點：480px、768px、1024px

## 5. 區塊架構確認
1. Hero
2. About
3. Skills
4. Education
5. Experience
6. Awards
7. Projects
8. Contact

## 6. 互動要求
- Anchor 點擊應平滑捲動
- TOC hover / active 可有 subtle 提示
- 卡片 hover 需帶微浮動與 glow

## 7. 交付物與流程
- 交付：`my-resume/index.html`
- 開發前先由你確認本規格
- 規格確認後，我僅在 `<style>` 區塊內調整 CSS

## 8. 確認事項
請確認以下內容是否符合預期：
1. 是否同意以 Apple Liquid Glass 風格為整體視覺方向？
2. 是否同意只改 `index.html` 的 `<style>` 區塊，不修改 HTML 結構？
3. 是否同意先確認此 `spec.md`，再進行實際 CSS 調整？

---

`spec.md` 已更新為 Apple Liquid Glass 風格確認稿，待你確認後再開始開發。