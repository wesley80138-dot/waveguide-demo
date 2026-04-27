# AR Waveguide Visualization Suite

**Modern Nanophotonics Lab**
PI: Prof. Yu-Chieh Cheng (鄭佑誠)
Department of Electro-Optical Engineering, National Taipei University of Technology (NTUT)

Lab website: <https://milu7751992.wixsite.com/modernphotonics>

---

互動式 AR 光波導擴瞳視覺化套件，6 個模組（3 個光線追跡 + 3 個 k-space 動量空間分析）。
本工具是實驗室「Augmented reality near-eye display」研究主題的教學/可視化工具。

## 檔案結構

```
waveguide-demo/
├── index.html                  ← 首頁 / 模組導覽（含實驗室與 PI 資訊）
├── simulator.html              ← Module 03 旗艦版完整模擬器
├── raytrace-incoupler.html     ← Module 01: In-coupler 光線追跡
├── raytrace-3gratings.html     ← Module 02: 3 道光柵完整路徑
├── kspace-1grating.html        ← Module 04: 單光柵 k-space
├── kspace-2gratings.html       ← Module 05: G1 + G2 k-space
├── kspace-3gratings.html       ← Module 06: G1 + G2 + G3 k-space
└── README.md
```

## 部署到 GitHub Pages

進到上傳頁：`https://github.com/wesley80138-dot/waveguide-demo/upload/main`

把更新過的 `index.html`（與這個 `README.md`）拖進去 commit，其他檔案沒變不用重傳。

`Settings → Pages` 確認 Source = `Deploy from a branch / main / (root)`，按 Save。

等 1–2 分鐘，網址生效：
`https://wesley80138-dot.github.io/waveguide-demo/`

## TODO（等實驗室 logo 與 NTUT 校徽檔案到位）

目前頁面用的是 SVG placeholder：
- 實驗室 logo：3 個重疊三角形的近似版本（在 affiliation bar、navbar、footer）
- NTUT：方框 + `NTUT` 文字徽記

收到正式檔後，找 index.html 內 `id="mnpl-mark"` 的 `<symbol>` 區塊與 `.ntut-bigmark` / `.ntut-mark .badge` 樣式換掉即可。
