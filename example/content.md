# 核心觀念：Vibe Coding 的洗鍊與留存
> ❝Vibe Coding 速度很快，但用完就丟的東西，永遠不會變成你的！❞

### 💡 為什麼需要模板化？
- **細節失控**：AI 生成的網頁很漂亮，但細節與架構很難手動調整
- **隨機性高**：每次生成結果都很隨機，風格、排版無法完全掌控
- **無法重複使用**：做完的東西通常是「免洗」的，下次需求又要從零開始

> **從免洗餐具到長期工具**
> 把 AI 隨機的輸出，變成可用 Markdown 維護的模板，並封裝成 Agent Skill 建立完整工作流。

---

# 1. 跨越工具的藩籬：工具能力培養
> 教學的目標不是強調節工具，而是了解如何解決痛點。

### 🛠️ 多工具交替使用的能力
- **不要被單一 AI 綁架**：工具間的差異沒想像中大，重要的是解決問題的思維。
- **避免長期合約**：最好用的 AI 一直在改變，靈活切換才是王道。
- **熟悉的環境**：不論是 VSCode, Cursor 還是 Antigravity，選擇一個順手的「工作區」開始。

---

# 2. 環境建置：為 AI Agent 鋪路
> 在開始 Vibe Coding 之前，先確保你的地基（環境）是穩固的。

### 📦 基礎軟體安裝
1. **Node.js**：推薦使用 [NVM](https://github.com/nvm-sh/nvm) 管理版本。
2. **Codex 安裝**：透過 npm 全域安裝 `@openai/codex`。
3. **工作區配置**：準備一個乾淨的資料夾作為 AI Agent 的工作範圍。

```prompt [label="安裝指令"]
# 安裝 NVM (Mac/Linux)
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.40.4/install.sh | bash

# 安裝 Node.js LTS
nvm install --lts

# 安裝 Codex
npm i -g @openai/codex
```

[tags]
- [green] 建議使用 nvm-windows (Windows 用戶)
- [blue] Codex 支援 ChatGPT 帳號或 API Key 登入
[/tags]

---

# 3. 實戰演練：從一觸即發到細節痛點
> 在終端機一句話生成網頁，是開始，也是挑戰。

### 🚀 快速生成初稿
- 使用明確的 Prompt 定義目標（單一 HTML、CSS/JS 內含）。
- 指定設計風格（例：日系清爽、漸層背景）。
- 規劃視窗架構（側邊欄目錄、社群連結）。

### ⚠️ Vibe Coding 的隱形陷阱
> **看起來可以用，但不代表好改。**
- **隨機性問題**：與 AI 對話調整細節時，常會動到原本滿意的部分。
- **維護成本高**：直接修改幾千行的 HTML 原始碼，對開發者來說極其痛苦。

---

# 4. 逆向工程：建立可維護的模板
> 既然輸出充滿隨機性，那就建立一套「Markdown 驅動」的穩定腳本。

### 🏗️ 模板化思維
- **拆解結構**：將網頁拆解為標題、列表、步驟、圖片、洞察框。
- **Markdown 定義**：使用約定的 Markdown 語法來維護「內容」。
- **即時編譯**：建立 `dev` 腳本，只要存檔 Markdown，網頁就即時更新。

```markdown
[flow]
1. 分析現有 HTML 結構
2. 定義對應的 Markdown 標記語法
3. 撰寫 build/dev 腳本
4. 實現 Markdown → HTML 的單向渲染
[/flow]
```

---

# 5. 進階：封裝為 Agent Skill
> 將你的工作流自動化，變成 AI 可以理解並執行的「技能」。

### 🧩 Skill 的核心要素
- **SKILL.md**：定義 Skill 的名稱、描述與觸發時機。
- **Scripts**：存放負責轉換、打包的程式碼。
- **References**：提供 Markdown 格式與 HTML 模板作為參考範例。

> **為什麼要封裝？**
> 你不再需要去背誦特殊語法，只需提出需求，AI 會自動辨識並幫你套用合適的版型。

---

# 6. 成就達成：部署與 OG 優化
> 讓你的講義網頁被全世界看見。

### 🌐 輕鬆部署到 GitHub Pages
- **Init & Push**：將專案推送到 GitHub。
- **GitHub Actions**：設定 Pages 自動部署。
- **SEO 與 Open Graph**：確保分享時有標題、描述與漂亮的縮圖。

[summary]
- 🏗️ **模板化** | 解決 Vibe Coding 細節難改的痛點
- ⚙️ **Agent Skill** | 將工作流系統化，降低工具使用門檻
- 🚀 **長期維護** | 讓 AI 輔助開發的成果從Demo走向產品
[/summary]

[bonus title="🎁 鼎淵的 Vibe Coding 建議"]
Vibe Coding 的價值不在於「快」，而在於「賦能」。

當你能把腦中的工作流編成一套系統時，你就不再只是工具的使用者，而是工具的設計者。
[/bonus]
