# AR Waveguide Pupil Expansion — Web Demo

互動式 AR 光波導擴瞳模擬器，含 3D 光線追跡、光柵效率調整、Eyebox 均勻度視覺化。

## 檔案結構

```
waveguide-demo/
├── index.html       ← 首頁（landing page，深色科技感）
├── simulator.html   ← 3D 模擬器本體（被首頁的 iframe 嵌入）
└── README.md
```

兩個 HTML 檔都是 self-contained（無任何外部 CDN 依賴），可直接放在任何靜態主機上。

---

## 部署到 GitHub Pages

### 步驟 1：上傳檔案

進到你的 repo 頁面（`https://github.com/wesley80138-dot/waveguide-demo`），因為是空 repo，畫面中間會有一段：

> Get started by **creating a new file** or **uploading an existing file**.

點 **`uploading an existing file`** 連結（或直接打開 `https://github.com/wesley80138-dot/waveguide-demo/upload/main`）。

把這三個檔案一起拖進上傳區：
- `index.html`
- `simulator.html`
- `README.md`

下面填 commit message（例如 `Initial site`），按 **Commit changes**。

### 步驟 2：啟用 GitHub Pages

1. Repo 頁面點 `Settings` → 左側 `Pages`
2. Source 選 `Deploy from a branch`
3. Branch 選 `main`，資料夾 `/ (root)`
4. 按 `Save`

### 步驟 3：等 1–2 分鐘

重新整理 Pages 設定頁，最上面會出現網址：

```
https://wesley80138-dot.github.io/waveguide-demo/
```

第一次載入打開的就是漂亮的首頁，3D 模擬器會以 iframe 嵌在中間。

---

## 之後想更新內容

直接在 repo 介面把對應的檔案重新上傳覆蓋（`Add file → Upload files`），網站會在 1–2 分鐘內自動更新。
