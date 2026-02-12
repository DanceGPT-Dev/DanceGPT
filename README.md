# DanceGPT：AI 視覺辨識桌面自動化輔助工具
### DanceGPT: An AI-Powered Desktop Interaction & Automation Assistant Tool
💾 **[DOWNLOAD Webpage](https://script.google.com/macros/s/AKfycbx9HXEn6j8M8CR8tQ8yTRFP1GhmDyUAzTwepc1WkF7n7KNeu_DwoLmiQcZbC16G0EH3/exec)**
<p align="left">
  <img src="https://i.imgur.com/4bW1LNO.gif" width="650" alt="DanceGPT Framework Visualization">
</p>

## 🛠️ 產品定位與使命
**DanceGPT** 是一套專為提升桌面操作效率而設計的**智慧型輔助工具**。本專案的使命在於透過可重複、可配置的自動化流程編排，協助使用者降低高頻率、機械化的操作負擔，讓使用者能將精力專注於更具創造性與核心價值的任務上。

---
## 📜 核心聲明與使用規範 (Core Disclaimer)

* **性質定義**：本專案定位為一套桌面輔助工具，旨在提供一個可觀測、可延展的互動自動化框架。
* **使用限制**：**本輔助工具僅限於個人辦公自動化實驗使用、技術交流及學術研究** 。
* **不具特定指向性**：本工具不指定用於任何特定軟體、遊戲或受版權保護之平台，開發初衷並非針對任何特定環境設計。
* **合法合規使用**：使用者須確保其使用行為符合當地法律法規、第三方平台之使用政策及 GitLab 可接受使用政策。開發團隊不對使用者之個人行為承擔法律責任。

---

## 🛒 收費資訊
訂單成立後，系統即會為您開通 DanceGPT 使用權限。

<img width="336" height="91" alt="image" src="https://github.com/user-attachments/assets/5eed68f0-1548-4b1c-88bb-0dbe55e1aa82" />


---

## 🏭 核心應用場景 (Application Scenarios)

DanceGPT 的設計初衷是為了解決各種軟體環境中「無 API 對接」時產生的機械化勞動：

### 1. 資料處理與行政庶務 (Data Entry)
* **資料格式轉換**：自動處理 PDF 與 Excel 間的欄位複製，避免人工搬運數千筆資料的疲勞與錯誤。
* **檔案批次命名**：自動化處理大量檔案的選取、重新命名與分類存檔。
* **網頁表單填寫**：協助將本地端資料庫資訊，逐筆輸入至舊式的 Web 管理後台。

### 2. 軟體測試與品質保證 (QA Testing)
* **壓力測試 (Stress Testing)**：模擬高頻率精確點擊，測試系統在高壓操作下的穩定性與崩潰邊界。
* **迴歸測試 (Regression Testing)**：在軟體更新後自動執行標準路徑，確保原有功能運作無誤。

### 3. 數位互動與資產管理 (Digital Interaction & Asset Management)
針對需要高度人工判斷或重複性視覺確認的任務：
* **互動推廣行為**：協助在社群平台執行定時的維護與互動行為，如自動回覆或社群參與。
* **數位資產保存**：精確執行「翻頁 -> 等待讀取 -> 截圖 -> 存檔」循環，協助研究者保存數位資料。

### 4. 專業設計軟體重複操作 (Design Automation)
* **影像處理**：在 Photoshop 等軟體中，對大量照片執行重複的濾鏡調整或批次加工。
* **CAD/3D 建模**：在場景佈置時，自動執行重複性的物件複製、平移及旋轉調整。

---

## 🧩 核心功能亮點 (Key Features)

### 🔌 物理級硬體交互 (HID Interface)
支援 **Arduino Leonardo** 等硬體裝置，透過實體 USB 接口發送物理鍵盤與滑鼠訊號。此技術確保了輸入訊號與真實硬體完全一致，提供最純淨、最真實的輔助體驗。

<p align="left">
  <img src="https://github.com/user-attachments/assets/0d99cb51-3a79-437d-ac6f-6daf2b49ed5b" width="600" alt="DanceGPT Hardware Architecture">
</p>

### 🕺 隨機化行為編排 (Probabilistic Workflow)
* **流程優化**：支援機率驅動的執行路徑，模擬人類操作的隨機特性，避免機械化執行。
* **高複雜度支援**：提供模組化設計，協助使用者處理高難度的長流程自動化實驗。

<p align="left">
  <img src="https://github.com/user-attachments/assets/1c0b2ca3-bcf6-45cf-a52d-a5bc44500a9f" width="600" alt="DanceGPT Script Logic Flowchart">
</p>


### 👁️ AI 視覺辨識輔助
整合先進的視覺追蹤與圖像特徵提取技術，實時監測螢幕狀態並根據預設邏輯作出動態反應，優化桌面操作的流暢度與穩定性。

### 🚨 遠端通報與自動化監控
* **執行狀態監測**：內建智慧監控機制，確保自動化流程在安全預期內運行。
* **即時通報**：整合 Discord Webhook，將執行日誌與異常狀態即時推送至行動端，達成遠端觀測。

---

## 🛠️ 技術架構與作動原理

1. **影像分析層**：利用高效比對算法掃描目標區域。
2. **邏輯調度層 (`Script_main.m`)**：負責檢查點（Checkpoint）掃描、異常偵測與狀態切換。
3. **行為執行層 (`Script_body.m`)**：定義具體動作路徑，並透過 `Keyboard_event` 和 `Mouse_event` 產生隨機操作。
4. **硬體輸出層**：將邏輯指令轉化為 USB 物理訊號輸出。

---

## 📘 開發者 API 說明

本框架提供標準化介面，供研究人員編排精確的互動行為：

### 1. 鍵盤操作：`Keyboard_event`
**用途**：模擬鍵盤按下與釋放動作。

* **參數說明**：
    * `press_or_release`: 指定按下 (`KEY.PRESS`) 或釋放 (`KEY.RELEASE`)。⚠️ 兩者應成對出現。
    * `key`: 指定按鍵（支援字母 `'A'-'Z'`、數字 `'0'-'9'`、功能鍵 `KEY.CTRL` / `KEY.ALT` / `KEY.SHIFT` 等）。
    * `min_time`, `max_time`: 按鍵持續或等待時間，由系統隨機取值（毫秒 ms）。
    * `fast_mode`: (可選) 帶入此參數時，該操作將與下個操作幾乎同步執行（適用於組合鍵）。

* **範例**：
    ```matlab
    % 按下 x 鍵持續 0.1 秒後釋放
    Keyboard_event(KEY.PRESS, 'x', 100, 100);
    Keyboard_event(KEY.RELEASE, 'x', 100, 100);

    % 同時按下 ALT + X 鍵
    Keyboard_event(KEY.PRESS, KEY.ALT, 0, 0, 0);
    Keyboard_event(KEY.PRESS, 'x', 100, 100);
    ```

### 2. 滑鼠操作：`Mouse_event`
**用途**：模擬滑鼠移動、點擊與釋放。

* **參數說明**：
    * `action`: 指定動作 (`MOUSE.MOVE`, `MOUSE.PRESS`, `MOUSE.RELEASE`)。
    * `varargin`: 
        * `MOVE` 時：傳入 `[X, Y]` 螢幕座標向量。
        * `PRESS/RELEASE` 時：傳入按鍵類型 (`MOUSE.LEFT_BUTTON`, `MOUSE.RIGHT_BUTTON` 等)。

* **範例**：
    ```matlab
    % 移動滑鼠至 (500, 300)
    Mouse_event(MOUSE.MOVE, [500, 300]);

    % 執行左鍵點擊
    Mouse_event(MOUSE.PRESS, MOUSE.LEFT_BUTTON);
    Time_pause_DanceGPT(0.1);
    Mouse_event(MOUSE.RELEASE, MOUSE.LEFT_BUTTON);
    ```

---

## ⚠️ 服務條款摘要 (Terms of Service)

* **設備綁定**：採一機一碼綁定機制，確保授權環境唯一。
* **隱私與安全**：本程式僅收集必要之運行數據以提升輔助品質，不外洩使用者個人隱私。

---

## 📩 聯絡我們

若您對此輔助工具有任何技術建議或問題，請聯繫開發團隊：
* **Email**: dancegpt0818@gmail.com

---
© DanceGPT. All Rights Reserved.
