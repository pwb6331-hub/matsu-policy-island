# 連江縣「老宅延壽機能復新計畫」政策島 3D 微縮城市探索

[![GitHub Pages](https://img.shields.io/badge/GitHub%20Pages-Live%20Demo-brightgreen?style=for-the-badge&logo=github)](https://pwb6331-hub.github.io/matsu-policy-island/)
[![WebGL](https://img.shields.io/badge/WebGL-Three.js_r160-blue?style=for-the-badge&logo=three.js)](https://threejs.org/)
[![License](https://img.shields.io/badge/License-連江縣政府工務處-orange?style=for-the-badge)](https://www.matsu.gov.tw)

> 🏛️ **線上展示網址（手機、平板、桌機皆可即刻連線）：**  
> 🔗 **[https://pwb6331-hub.github.io/matsu-policy-island/](https://pwb6331-hub.github.io/matsu-policy-island/)**

---

## 🏝️ 專案簡介與 3F 造島思維

本系統以**「3F 造島思維」**（Free-Form Procedural World Generation）為核心，不依賴預先打包的第三方龐大模型，而是運用純數學幾何（Primitive Geometries）、演算法與空間座標系統，將連江縣「四鄉五島」拆解為 AI 可計算、可施工的微縮城市（Tilt-Shift Diorama）：

1. **南竿示範島**：福澳港碼頭、貨運吊臂、媽祖巨神像地標、4～6 層連棟公寓示範群（增設透明景觀電梯、外掛管線安全整理、屋頂綠能防水隔熱拉皮）。
2. **北竿芹壁島**：依山傍海的傳統芹壁石屋聚落，具備花崗岩「人字砌」、「丁字砌」質感，鮮明朱紅起翹「馬鞍形封火山牆」與屋頂「壓瓦石」防颱工藝保留。
3. **東引燈塔島**：國之北疆海蝕峭壁，18 世紀歐風白磚燈塔（具備 360 度動態旋轉探照光束），示範抗強陣風與鹽霧侵蝕之外部管線不鏽鋼夾具固定工法。
4. **莒光樂活島**：東莒白犬燈塔、大埔聚落，示範銀髮友善居家在宅安心安老無障礙緩坡道、防滑扶手與高齡弱勢加碼 30 萬全額保障。
5. **海洋與船舶動態**：即時頂點正弦波浪（Vertex Waves）、穿梭航行於四鄉五島的「臺馬之星」與「南北之星」客輪、白晝/夕陽/夜景三時相光影切換，以及純 Web Audio 演算法合成的海潮浪花音效。

---

## 📂 檔案資料獨立存放目錄架構 (Standalone Data Directory)

本儲存庫遵循使用者要求，將所有法規、表單、手冊與數據資料**單獨存放**，任何人或外部系統皆可獨立下載與調用：

```tree
matsu-policy-island/
├── index.html                           # 3D 互動微縮政策島主網頁 (GitHub Pages 部署檔)
├── README.md                            # 專案說明與連線指引
│
├── data/                                # 📊 原始數據資料庫 (JSON 格式)
│   ├── agencies_32.json                 # 全台及離島 32 家耐震結構初評專業機構名錄
│   ├── qa_50.json                       # 官方老宅延壽宣傳手冊 50 題 Q&A 全題庫
│   └── scenarios_40.json                # 40 組情境補助試算手冊精準數據
│
├── docs/                                # 📑 官方指導手冊與折頁文宣 (PDF)
│   ├── 老宅延壽宣傳手冊_20261013_修正2版.pdf
│   ├── 老宅延壽宣傳手冊_折頁雙面三折.pdf
│   └── 老宅延壽計畫補助情境手冊_1151027.pdf
│
├── forms/                               # 📄 官方 6 大申請表格 (Word docx 格式)
│   ├── 1-修繕需求申請表(透天住宅類).docx
│   ├── 2-申請補助自我評估表(透天住宅類).docx
│   ├── 3-修繕需求申請表(公寓類).docx
│   ├── 4-申請補助自我評估表(公寓類).docx
│   ├── 5-申請補助計畫書(透天住宅類).docx
│   └── 6-申請補助計畫書(公寓類).docx
│
├── images/                              # 🖼️ 流程圖與行動 QR Code (JPG)
│   ├── qrcode_matsu_gov.jpg             # 連江縣政府老宅延壽專區 QR Code
│   └── old_house_registration_flow.jpg  # 舊有房屋證明及地政第一次測量登記全流程圖
│
└── presentation/                        # 📊 官方政策簡報 (PPTX)
    └── 115年度連江老宅簡報_公版(1151013修正定稿版).pptx
```

---

## 🧮 補助計算核心：三取小嚴格比對機制

系統內建符合內政部國土管理署及連江縣政府標準之試算核心：

$$\text{核定補助款} = \min\Big(\text{合約總工程款 (A)} \times 65\%,\; \text{施作面積} \times 3,500\text{元/㎡},\; \text{法定單項上限}\Big)$$

- **法定單項天花板**：
  - 增設電梯：最高 400 萬元
  - 外牆立面修繕：公寓最高 300 萬元；透天依樓層 100 萬～300 萬元
  - 屋頂防水隔熱：公寓最高 150 萬元；透天最高 20 萬元
  - 公共管線修繕：公寓最高 200 萬元；透天最高 30 萬元
- **高齡弱勢加碼**：室內專有部分一般戶最高 20 萬元；戶內設籍 65 歲以上長輩或弱勢族群直接**加碼至 30 萬元全額補助保障**。

---

## 📞 諮詢窗口與服務專線

- **主辦單位**：連江縣政府工務處 都市計畫建築管理科
- **駐府輔導**：福建金門馬祖地區建築師公會 駐府輔導服務台
- **服務專線**：**(0836) 25330 分機 6338**
- **服務地址**：連江縣南竿鄉介壽村 76 號 3 樓
- **官方網站**：[連江縣政府全球資訊網](https://www.matsu.gov.tw)
