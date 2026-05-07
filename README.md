# DIY-CNC
Repurposing a legacy 3D printer into a functional CNC machine. By upgrading the original 3-axis frame to handle high-load and high-noise (EMI) environments.
這是一份完整彙整後的 GitHub README 硬體章節。我已依照你的要求，統一使用 `###` (標題) 與 `*` (列點) 符號，並將 **Manta E3EZ**、**CB1**、**Sensorless Homing** 以及 **ZK-BM1** 等關鍵硬體完整加入：

### 1. 核心控制系統 (Control System)
* **主控板 (MCU)：** 採用 **BigTreeTech Manta E3EZ**，專為整合與穩定性設計，提供優異的運動控制性能。
* **核心運算 (SoC)：** 搭載 **BTT CB1** 模組運行 Klipper 韌體，透過板對板連接省去 USB 線路，大幅降低數據傳輸干擾與震動風險。
* **散熱管理：** 配置主動式風扇直吹驅動模組與 SoC，確保在高強度切削任務中，系統不會因過熱導致運算延遲。

### 2. 馬達與歸零模式 (Motors & Homing)
* **步進驅動器：** 使用 **BTT EZ2209**，具備靜音驅動與高精度的電流回饋能力。
* **歸零技術：** 採用 **Sensorless Homing (無限位器歸零)** 模式，利用 TMC 驅動器的 StallGuard 技術達成精確定位。
* **硬體簡化：** 透過無限位器設計，有效減少機架佈線複雜度，並徹底解決 CNC 加工環境下粉塵堆積導致限位開關損壞的問題。

### 3. 主軸系統整合 (Spindle Integration)
* **驅動核心：** 採用 **ZK-BM1 直流馬達驅動板**，專責處理主軸馬達的高電流負載，確保切削時的扭力輸出穩定。
* **控制模式：** 透過 Manta E3EZ 的 **PWM 接口** 對接 ZK-BM1 訊號輸入，實現由 Klipper 韌體控制的**數位化轉速調節**與啟停功能。
* **物理隔離：** 主軸動力系統（ZK-BM1 與專屬電源）與主控制電路採物理分離佈置，保持 15cm 以上距離，防止直流馬達的高頻雜訊與磁場干擾 MCU 訊號。

### 4. 電氣防護與安全性 (EMI & Safety)
* **EMI 雜訊抑制：** 於總電源輸入端加裝工業級 **EMI 濾波器**，並針對主軸與馬達線路採用**金屬屏蔽線**，有效隔離電磁干擾。
* **接地方案：** 實施全機等電位接地與屏蔽層單端接地，防止加工產生的靜電積累。
* **緊急安全保護：** 配置實體 **緊急停止開關 (E-Stop)**，並結合 Klipper 韌體邏輯與馬達堵轉偵測 (Stall Detection)，提供多層次的硬體安全防護。
