# 🎨 高質感 Web 製作規範 (Vibe Coding 結構版)

這是一份用於指導 AI 或開發團隊製作具備高級感、流暢互動與清晰結構的網頁設計系統。它包含三個版本：精簡版、完整版、模板版。

---

## 🔹 一、精簡版（約 300–400 字）

適合直接複製貼上，作為對 AI 的快速設計指令。

⸻

### 【Web 製作技術規格】

請按照以下原則製作頁面：

**1. 布局結構 (Layout & Structure)**
- **核心布局**: 使用 **Magazine Layout** (雜誌式排版)，避免內容區塊平均分布。
- **視覺層級**: 強調標題 (H1/H2) 與圖片的尺寸對比，保留大面積留白 (Whitespace)。
- **視線動線**: 採用 **Z-Pattern** 或 **F-Pattern** 視線動線來安排資訊優先順序。

**2. 動效設計 (Motion & Narrative)**
- **區塊入場**: 所有內容區塊使用 **Reveal on Scroll** (滾動時淡入 + 輕微上浮)。
- **背景效果**: 背景可加入 **Parallax Scrolling** (視差滾動)，速度設定為前景的 50%。
- **滾動敘事**: 支援 **Scrollytelling** (滾動分段動畫)，將複雜資訊拆解為隨滾動觸發的步驟。

**3. 質感控制 (Texture & Visuals)**
- **背景紋理**: 漸層或單色背景疊加一層細微的 **Grain Texture** (顆粒紋理)，避免過度平滑的塑膠感。
- **載入體驗**: 使用 **Skeleton Screen** (骨架屏) 取代空白等待畫面，提升感知效能。

**4. 交互回饋 (Interaction & Feedback)**
- **微交互**: 所有可點擊元素加入 **Micro-interactions** (例如 Hover 時輕微放大 `scale(1.03)` 並增強陰影)。
- **操作通知**: 操作完成後使用 **Toast Notification** (黑底白字、圓角、從底部或頂部滑入) 進行非阻斷式提示。

**5. 流程設計 (Flow & State)**
- **用戶引導**: 為新用戶加入多步驟的 **Onboarding Flow** (引導流程)，每一步都有清晰的進度指示。
- **空狀態**: 設計 **Empty State** (空狀態) 頁面，包含引導性插圖與明確的行動呼籲 (Call to Action)。
- **頁面轉場**: 使用 **Seamless Page Transitions** (平滑轉場)，例如淡入淡出或滑動，避免頁面刷新時的白屏閃爍。

⸻

## 🔹 二、完整版（約 900–1200 字）

這是一份更詳細的、可作為團隊內部設計系統或 AI 系統級指令的版本。

⸻

### 【高質感 Web 製作規範 v1.0 (Vibe Coding 結構版)】

請嚴格依照以下設計系統與技術規範開發所有頁面，以確保產品具備清晰的空間秩序、可感知的時間節奏、明確的回饋機制與高級而不浮誇的視覺質感。

#### 一、布局與結構 (Layout & Structure)

- **核心布局模式**: 優先採用 **Magazine / Editorial Layout** (雜誌或編輯式排版)。強調標題、段落與圖片之間的不對稱、交錯式排版，創造視覺張力。
- **視覺層級 (Visual Hierarchy)**: 嚴格遵守清晰的視覺層級。H1 應為頁面最突出的視覺焦點，其次是 H2，最後是內文 (Body)。字體大小、粗細與顏色對比是實現層級的主要手段。
- **留白 (Whitespace)**: 避免將元素平均對齊或填滿整個畫面。保留大面積的留白，用以分隔不同區塊、引導視線、並營造高級感與呼吸感。
- **視線動線 (Scan Path)**: 根據內容的重要性，主動設計用戶的閱讀路徑。對於資訊探索頁，採用 **Z-Pattern**；對於內容密集的文章或列表頁，採用 **F-Pattern**。
- **特殊布局**: 若內容具有時間順序性（例如公司發展史、項目進程），應採用 **Timeline Layout** (縱向時間軸) 進行敘事，增強故事感。

#### 二、動效與敘事 (Motion & Narrative)

- **入場動畫 (Entrance Animation)**: 所有非首屏的內容區塊，統一加入 **Reveal on Scroll** 動畫。當區塊進入可視範圍時，從 `opacity: 0` 淡入至 `opacity: 1`，並伴隨一個 `transform: translateY(10px)` 到 `translateY(0)` 的輕微上浮效果。動畫時長約 0.5-0.8 秒，使用 `ease-out` 曲線。
- **視差滾動 (Parallax Scrolling)**: 若頁面有背景圖片或大型視覺元素，應加入視差滾動效果。背景元素的滾動速度應設定為前景內容滾動速度的 **50%**，以創造深度感。
- **滾動敘事 (Scrollytelling)**: 對於需要分步解釋的複雜概念或產品特性，必須支援 Scrollytelling 結構。將一個長篇故事拆解為多個視覺場景，隨著用戶的滾動逐步觸發動畫、高亮特定文本、或切換圖表狀態。
- **頁面轉場 (Page Transitions)**: 應用程式內的所有頁面切換都必須是 **Seamless (無縫的)**。避免瀏覽器預設的白屏刷新。推薦使用 **Cross-fade** (交叉淡入淡出) 或 **Slide** (滑動) 轉場動畫，時長約 300-400ms。
- **載入狀態 (Loading State)**: 在等待數據或圖片載入時，必須使用 **Skeleton Screen** (骨架屏) 作為佔位符。骨架屏的形狀應模擬最終內容的佈局，並可加入微弱的脈衝或掃光動畫，以告知用戶系統正在處理中。

#### 三、質感與視覺 (Texture & Visuals)

- **背景紋理 (Grain Texture)**: 為避免大面積色塊或漸層顯得過於平滑和廉價，應在最底層疊加一層細膩、半透明的 **Grain Texture** (顆粒紋理)。紋理的強度應非常微弱，僅在特定角度和光線下可感知，旨在增加視覺深度。
- **陰影與模糊 (Shadow & Blur)**: 陰影應使用柔和、多層次的 **Soft Shadow**，避免使用單一、生硬的實色陰影。可適度使用 **Glassmorphism** (玻璃擬態) 效果，透過背景模糊 (`backdrop-filter: blur(10px)`) 創造毛玻璃質感。
- **色彩策略 (Color Strategy)**: 保持色彩使用的**節制性**。選擇一個主色、一個輔色和一個強調色。避免使用過度飽和的顏色，優先選擇略帶灰度的色調以提升高級感。
- **焦點強化 (Focus Enhancement)**: 主要的行動呼籲 (CTA) 按鈕和需要用戶關注的核心區塊，應使用與周圍環境形成**強烈對比**的顏色或尺寸，確保其在視覺上脫穎而出。

#### 四、交互與回饋 (Interaction & Feedback)

- **微交互 (Micro-interactions)**: 所有可點擊的元素（按鈕、連結、卡片等）必須包含微交互，以提供即時的物理回饋。
  - **Hover (懸停)**: 元素尺寸放大 **1.02 至 1.05 倍**，同時陰影應變得更深、更廣。
  - **Active (點擊時)**: 元素尺寸縮小至 **0.98 倍**。
  - **Transition (過渡)**: 所有狀態變化的過渡動畫時長應在 **150-250ms** 之間，使用 `ease-out` 曲線。
- **通知機制 (Notification System)**: 對於非關鍵性的操作成功或失敗提示，統一使用 **Toast Notification**。樣式為黑底白字、圓角矩形，從螢幕底部或頂部滑入，停留 3-5 秒後自動滑出。避免使用阻斷用戶流程的 Modal (模態框)。
- **空狀態設計 (Empty States)**: 必須為所有可能出現空數據的頁面（如空購物車、無搜索結果、零訊息）設計專門的空狀態。空狀態頁面應包含一個與品牌風格一致的**插圖**、一段友好的**引導文案**和一個明確的**行動呼籲按鈕** (例如「去逛逛」、「換個關鍵詞試試」)。
- **引導流程 (Onboarding Flow)**: 對於首次使用產品或進入複雜功能區的用戶，應設計一個**多步驟的 Onboarding Flow**。流程中必須有清晰的**進度指示器** (例如步驟條或分頁點)，並允許用戶隨時跳過。

#### 五、產品感知目標 (Product Perception Goals)

最終交付的頁面應讓用戶在無意識中感受到：
- **清晰的空間秩序**: 知道自己在哪里，要去哪里。
- **可感知的時間節奏**: 互動與等待都在預期之內。
- **明確的回饋機制**: 每次操作都有對應的響應。
- **高級的視覺質感**: 感覺產品精緻、可靠，而非廉價或粗糙。

⸻

## 🔹 三、架構師模板版

這是一個高度壓縮的、結構化的模板，用於快速定義一個新頁面或組件的「Vibe」。未來只需要填寫關鍵詞即可。

⸻

```yaml
# ---------------------------------------------------
#  Vibe Coding Specification - Template v1.0
# ---------------------------------------------------

# 1. Layout & Structure
#   - Core: [Magazine | Grid | List | Timeline]
#   - Hierarchy: [Strong | Medium | Weak]
#   - Whitespace: [Generous | Balanced | Compact]
#   - Scan Path: [Z-Pattern | F-Pattern | Free]

# 2. Motion & Narrative
#   - Entrance: [Reveal on Scroll | Fade In | Slide In]
#   - Scrolling: [Parallax | Scrollytelling | Static]
#   - Page Transition: [Cross-fade | Slide | None]
#   - Loading: [Skeleton | Spinner | Progress Bar]

# 3. Texture & Visuals
#   - Background: [Grain Texture | Gradient | Solid]
#   - Style: [Flat | Glassmorphism | Neumorphism]
#   - Shadow: [Soft | Hard | None]
#   - Color Palette: [Monochromatic | Analogous | Complementary]

# 4. Interaction & Feedback
#   - Micro-interaction: [Scale & Shadow | Color Change | Underline]
#   - Notification: [Toast | Snackbar | Modal]
#   - Empty State: [Illustration + CTA | Text Only]
#   - Onboarding: [Multi-step Modal | Tooltips | None]

# 5. Product Perception Goals
#   - Primary Goal: [Clarity | Efficiency | Elegance | Playfulness]
#   - Feeling: [Professional | Friendly | Minimalist | Bold]

# ---------------------------------------------------
#  Example for a Portfolio Website
# ---------------------------------------------------

# Layout:
#   Core: Magazine
#   Hierarchy: Strong
#   Whitespace: Generous
#   Scan Path: Z-Pattern

# Motion:
#   Entrance: Reveal on Scroll
#   Scrolling: Parallax
#   Page Transition: Cross-fade
#   Loading: Skeleton

# Texture:
#   Background: Grain Texture
#   Style: Flat
#   Shadow: Soft
#   Color Palette: Monochromatic

# Feedback:
#   Micro-interaction: Scale & Shadow
#   Notification: Toast
#   Empty State: Illustration + CTA
#   Onboarding: None

# Goal:
#   Primary Goal: Elegance
#   Feeling: Professional, Minimalist

```
