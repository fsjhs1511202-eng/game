# 🎯 CyberPulse Game Hub - 賽博脈衝 3D 戰術練槍與身法訓練平台
![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)
![Engine: Three.js](https://img.shields.io/badge/3D_Engine-Three.js_r128-00f3ff.svg)
![Styling: TailwindCSS](https://img.shields.io/badge/Styling-TailwindCSS-06b6d4.svg)
![WebRTC: PeerJS](https://img.shields.io/badge/P2P-PeerJS-purple.svg)
![Audio: Suno AI](https://img.shields.io/badge/BGM-Suno_AI_v3.5-pink.svg)
> **CyberPulse Mega Dojo** 是一款專為 FPS 電競玩家設計的三維槍法與 **WASD 身法急停（Counter-Strafe）** 瀏覽器訓練平台。融合 Three.js 3D 輕量化渲染、Valorant eDPI 靈敏度換算、16 款交錯訓練菜單與 P2P 區網 1v1 對決模式。
---
📌 目錄 (Table of Contents)
💡 專案緣由與動機
🎮 遊戲核心特色
🚀 16 大戰術訓練關卡庫
🛠 系統架構與開發歷程
🎵 Suno AI 主題曲音效
📦 快速開始與使用說明
📄 開源授權
---
💡 專案緣由與動機
🎯 緣由
在熱門第一人稱射擊遊戲（如《無畏契約 Valorant》、《反恐精英 CS2》、《Apex 英雄》）中，玩家的勝負往往取決於 「毫秒級的反應速度」 與 「急停（Counter-Strafe）射擊的精準度」。然而，市面上的練槍軟體多數需要下載龐大安裝包，或僅專注於「定點甩槍」，忽視了實戰中「一邊走位一邊對槍」的身法需求。
🚀 動機
為了提供玩家一個 零延遲、免下載、打開瀏覽器即可訓練 的高質感終端，本專案運用 Three.js WebGL 引擎 與 Web Audio API，打造出結合身法物理、第一人稱槍械視覺與沉浸式 Cyberpunk 氛圍的一站式練槍平台。
---
🎮 遊戲核心特色
🎯 WASD 走位與 AD 急停物理：真實還原移動時準心散開、急停瞬刻達到 100% 精準度的射擊體驗。
🔫 第一人稱武器裝備庫 (Viewmodels)：內建 Sheriff 警長手槍、Vandal 步槍、Stinger 衝鋒槍與 Operator 狙擊槍，搭配動態槍口火光與後座力反饋。
⚡ Valorant eDPI / CM360° 換算：支援客製化靈敏度，與熱門電競遊戲 hand-feel 完美相容。
🎨 2D Vector Crosshair Studio：提供顏色、長度、粗細與間距的自訂準心系統。
🌐 P2P 區網 1v1 槍法對決：透過 WebRTC / PeerJS 實現 4 位數簡化房號對決，支援即時分數與位置同步。
---
🚀 16 大戰術訓練關卡庫
平台採用 「靜態槍法 ↔ 走位戰術」 交錯穿插的排列，維持高節奏與耐玩度：
關卡	模式名稱	類型	訓練重點
01	Gridshot 3x3	🎯 靜態甩槍	網格三目標快點，鍛鍊手眼協調與極速定位
02	Smooth Tracking	🚶 走動跟槍	目標雙向動態走位，練習移動中平滑追蹤
03	Counter-Strafe AD	🚶 走動急停	模擬 Valorant 實戰拉槍對決與 AD 急停
04	Micro Precision Pixel	🎯 靜態點射	極小像素標靶，訓練高倍率遠距離爆頭
05	Vertical Bounce Track	🎯 垂直跟槍	目標沿 Y 軸彈跳，鍛鍊垂直控鼠能力
06	360° Wide Angle Reflex	🎯 廣角反應	四周隨機生成標靶，鍛鍊背身與大轉角定位
07~15	Tactical Combo Drills	🎯/🚶 綜合菜單	包含跳射、掩體閃角、連噴壓槍控槍等專項練習
16	Cyber Titan Boss Raid	🐉 魔王戰	巨型賽博泰坦 Boss 戰，考驗綜合走位與總輸出火力
---
🛠 系統架構與開發歷程
```
CYBERPULSE GAME HUB
├── index.html               # 3D Aim Trainer 主程式引擎 (Three.js + Controls)
├── cover.html               # 3D 展廳互動封面 (Interactive Hero & Audio)
├── hub.html                 # 平台介紹與 Native 3D 模擬試玩區
└── suno_theme_song.md       # Suno AI 主題曲提示詞指南
```
📈 開發歷程 (Development Timeline)
Phase 1 • 核心引擎建構：採用 Three.js R128 搭建 PerspectiveCamera 與 Yaw/Pitch 控制器，實作 Valorant eDPI 轉換與 2D 準心 Studio。
Phase 2 • 武器與急停物理：導入 WASD 第一人稱視角步伐晃動，建立射擊彈道與 AD 急停精準度判定機制。
Phase 3 • 關卡與 Titan Boss：規劃 16 款高強度交錯關卡，研發第 16 關具備護盾防禦機制的賽博泰坦 Boss。
Phase 4 • 音效與 P2P 連線：結合 Web Audio API 自研打擊音效，運用 PeerJS 導入 4 位數簡化房號區網 P2P 對決。
---
🎵 Suno AI 主題曲音效
專案配樂採用 Suno AI v3.5 創作主題曲 《CyberPulse: Lock and Strike》：
風格標籤：`Cyberpunk OST`, `Industrial Synthwave`, `Hard Dark EDM`, `Heavy Brass Horn`, `135 BPM`
音效整合：內建自研 Web Audio 合成器，可在無外部音檔加載狀況下產生重低音 Kick 與打擊雷射槍聲。
---
📦 快速開始與使用說明
本專案採用 Pure Front-End (純前端) 輕量架構，無需安裝額外的 Node.js 或後端服務：
複製專案庫 (Clone Repository)：
```bash
   git clone https://github.com/your-username/cyberpulse-game-hub.git
   cd cyberpulse-game-hub
   ```
啟動頁面：
打開 `hub.html`：檢視一頁式平台介紹與內建 3D 試玩。
打開 `index.html`：直接進入 3D Aim Trainer Pro 主訓練場。
打開 `cover.html`：體驗 3D 互動封面與主題曲試聽。
---
📄 開源授權
本專案採用 MIT License 授權條款，歡迎自由學習、修改與延伸開發！
