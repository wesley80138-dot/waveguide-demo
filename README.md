# AR Waveguide Lab — Interactive 3D Visualization Suite

互動式 AR 光波導擴瞳視覺化套件，包含 6 個模組：3 個光線追跡 + 3 個 k-space 動量空間分析。

## 檔案結構

```
waveguide-demo/
├── index.html                  ← 首頁 / 模組導覽（深色科技感）
│
├── simulator.html              ← Module 03 旗艦版完整模擬器
│                                  (Ray Tracing + 5-zone Efficiency + Eyebox 9 宮格)
│
├── raytrace-incoupler.html     ← Module 01: In-coupler 光線追跡（最簡）
├── raytrace-3gratings.html     ← Module 02: 3 道光柵完整路徑
│
├── kspace-1grating.html        ← Module 04: 單光柵 k-space
├── kspace-2gratings.html       ← Module 05: G1 + G2 k-space
├── kspace-3gratings.html       ← Module 06: G1 + G2 + G3 k-space
│
└── README.md
```

所有 HTML 檔都是 self-contained，無外部 CDN 依賴。

---

## 部署到 GitHub Pages

### 增量更新（你目前的情況）

你 repo 裡已經有舊版的 `index.html` + `simulator.html` + `README.md`。現在要做的是：

1. **覆蓋 index.html、README.md，加入 5 個新檔案**

   打開上傳頁：
   ```
   https://github.com/wesley80138-dot/waveguide-demo/upload/main
   ```

   把這個資料夾裡的這 7 個檔案**全部**拖進去：
   - `index.html`（會覆蓋舊的）
   - `README.md`（會覆蓋舊的）
   - `raytrace-incoupler.html`（新）
   - `raytrace-3gratings.html`（新）
   - `kspace-1grating.html`（新）
   - `kspace-2gratings.html`（新）
   - `kspace-3gratings.html`（新）

   `simulator.html` 不用重新上傳（內容沒變）。

2. **填 commit message**（例如 `Add k-space modules and ray-tracing variants`）→ Commit changes。

3. **等 1–2 分鐘**，重新整理：
   ```
   https://wesley80138-dot.github.io/waveguide-demo/
   ```

   如果看到的還是舊版，按 `Ctrl + F5` 強制重新整理瀏覽器 cache。

---

## 模組導覽

| Module | 檔名 | 說明 |
|--------|------|------|
| 01 | `raytrace-incoupler.html` | 單一 In-coupler + TIR 全反射，最簡示範 |
| 02 | `raytrace-3gratings.html` | G1 + G2 + G3 完整 3D 光線追跡 |
| 03 ★ | `simulator.html` | 旗艦版：含 5-zone 效率、Eyebox 9 宮格、BTM 均勻度 |
| 04 | `kspace-1grating.html` | 9 個 FOV 點在 In-coupler 上的 k-space 分布 |
| 05 | `kspace-2gratings.html` | G1 + G2 的 k-space 演化（m=0, +1 階） |
| 06 | `kspace-3gratings.html` | G1 + G2 + G3 完整 k-space pipeline |

首頁 (`index.html`) 會以卡片畫廊的方式呈現所有模組，點擊後在新分頁開啟對應的 HTML。
