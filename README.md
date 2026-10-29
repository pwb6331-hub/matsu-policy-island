# 連江縣「老宅延壽機能復新計畫」3D 互動政策群島

[![GitHub Pages](https://img.shields.io/badge/GitHub%20Pages-Live%20Demo-brightgreen?style=for-the-badge&logo=github)](https://pwb6331-hub.github.io/matsu-policy-island/)
[![WebGL](https://img.shields.io/badge/WebGL-Three.js-blue?style=for-the-badge&logo=three.js)](https://threejs.org/)
[![License](https://img.shields.io/badge/License-連江縣政府工務處-orange?style=for-the-badge)](https://www.matsu.gov.tw)

> 🏛️ **線上展示網址（手機、平板、桌機皆可即刻連線）：**  
> 🔗 **[https://pwb6331-hub.github.io/matsu-policy-island/](https://pwb6331-hub.github.io/matsu-policy-island/)**

---

## 🏝️ 專案特色

本系統為連江縣「老宅延壽機能復新計畫」專屬 3D 互動政策城市，以四座微縮政策島嶼（南竿、北竿、東引、莒光）串聯航線，結合微縮模型感與懸浮資訊展板：

- **南竿示範島**：福澳港腹地碼頭、媽祖巨神像地標立柱、4～6 層連棟公寓示範聚落（外掛透明景觀電梯、屋頂綠能防水隔熱拉皮）。
- **北竿芹壁島**：芹壁花崗岩石屋聚落，具備人字砌、丁字砌岩石色澤與紅色馬鞍形封火山牆，壓瓦石防颱傳統工法保存。
- **東引燈塔島**：國之北疆峭壁，歐風百年白磚燈塔，示範強陣風防風外部電氣與給排水管線固定工法。
- **莒光樂活島**：東莒白犬燈塔、大埔聚落，示範銀髮友善在宅安心安老無障礙緩坡道、防滑扶手與高齡弱勢加碼 30 萬。

---

## 📂 檔案資料獨立存放目錄 (Standalone Data Directory)

本儲存庫遵循資料獨立原則，將所有法規、表單、手冊與數據資料**單獨存放**於專屬目錄中，隨時可獨立下載與調用：

```tree
matsu-policy-island/
├── index.html                           # 3D 互動政策島主網頁 (手機/平板/桌機直接連線)
├── README.md                            # 專案指南與連線說明
│
├── data/                                # 📊 原始數據資料庫 (JSON 格式)
│   ├── agencies_32.json                 # 32 家耐震結構初評機構完整名冊
│   ├── qa_50.json                       # 官方宣傳手冊 50 題 Q&A 全題庫
│   └── scenarios_40.json                # 40 組情境補助試算手冊數據庫
│
├── docs/                                # 📑 官方指導手冊與折頁文宣 (PDF 格式)
│   ├── 老宅延壽宣傳手冊_20261013_修正2版.pdf
│   ├── 老宅延壽宣傳手冊_折頁雙面三折.pdf
│   └── 老宅延壽計畫補助情境手冊_1151027.pdf
│
├── forms/                               # 📄 官方 6 大標準申請表格 (Word docx 格式)
│   ├── 1-修繕需求申請表(透天住宅類).docx
│   ├── 2-申請補助自我評估表(透天住宅類).docx
│   ├── 3-修繕需求申請表(公寓類).docx
│   ├── 4-申請補助自我評估表(公寓類).docx
│   ├── 5-申請補助計畫書(透天住宅類).docx
│   └── 6-申請補助計畫書(公寓類).docx
│
├── images/                              # 🖼️ 流程圖與行動 QR Code (JPG 格式)
│   ├── qrcode_matsu_gov.jpg             # 連江縣政府老宅延壽專區 QR Code 原圖
│   └── old_house_registration_flow.jpg  # 舊有房屋證明及地政第一次測量登記全流程圖
│
└── presentation/                        # 📊 官方公版政策簡報 (PPTX 格式)
    └── 115年度連江老宅簡報_公版(1151013修正定稿版).pptx
```

---

## 📞 諮詢窗口與服務專線

- **主辦單位**：連江縣政府工務處 都市計畫建築管理科
- **駐府輔導**：福建金門馬祖地區建築師公會 駐府輔導服務台
- **服務專線**：**(0836) 25330 分機 6338**
- **服務地址**：連江縣南竿鄉介壽村 76 號 3 樓
- **官方網站**：[連江縣政府全球資訊網](https://www.matsu.gov.tw)
