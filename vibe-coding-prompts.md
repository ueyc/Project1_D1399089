# Vibe Coding 指令說明｜東協不邪影展專題網站

- 作者：D1399089 吳宜蓁
- 課程：1151 數位行銷程式設計 Project 1
- 工具：Claude（對話式 AI）＋ GitHub ＋ Vercel ＋ InfinityFree
- 主題：《新中城．城中心》影展企劃書「東協不邪」

## 我下的 Prompt

### Prompt 1：提供需求與素材
> 依照題目指令完成作業內容：影展專題介紹。題目「東協不邪」（請閱讀企劃書了解），圖片使用圖3。（附上作業要求截圖、企劃書 docx、照片）

**目的：**讓 AI 讀懂課程規格（導覽列、側邊欄、分頁、SEO、Grid、RWD、CSS 分檔、images 資料夾）與企劃書內容。

### Prompt 2：規格拆解（由 AI 對照作業要求執行）
| 作業要求 | 實作方式 |
|---|---|
| 導覽列、側邊欄、分頁 | 7 個 HTML 頁面，頂部導覽列＋每頁左（右）側章節側邊欄 |
| SEO | title、meta description／keywords、Open Graph、canonical、JSON-LD、sitemap.xml、robots.txt、圖片 alt、語意化標籤 |
| Grid System | `css/grid.css` 12 欄 Grid（`.row`、`.col-*`） |
| RWD | `css/responsive.css`，900px 以下側邊欄堆疊、導覽列變漢堡選單 |
| CSS 切割 | `base / grid / layout / components / responsive` 五個檔案放在 `css/` |
| 圖片資料夾 | 所有圖片放在 `images/` |

### Prompt 3：內容轉譯
> 將企劃書的執行摘要、現況分析、SWOT、市場區隔、定位、問卷、創意聯想、故事腳本與分鏡，重新整理成網頁能閱讀的段落、卡片與表格，不要整份複製貼上。

### Prompt 4：視覺風格
> 以東協廣場泰式菜單照片的暖橘、奶油色與綠色為主色，風格親切、有食物的溫度。

### 後續調整（可依實際對話補充）
- 「首頁大圖太暗，請調整文字對比」
- 「手機版選單改成可展開」
- 「把 canonical／sitemap 的網址換成我的 Vercel 網址」

## 我的反思
1. 先把作業規格逐條貼給 AI，成果比只說「做網站」精準。
2. AI 能快速做出結構，但內容正確性（數據、引用）仍須對照企劃書人工確認。
3. 版面要實際用手機與電腦檢查 RWD。

## 部署
1. 上傳專案至 GitHub repository
2. Vercel Import GitHub repo 部署（純靜態，無需 build）
3. 以 FTP／檔案管理員上傳同一份檔案至 InfinityFree `htdocs/`，取代預設首頁
