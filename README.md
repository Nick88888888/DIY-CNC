### 1. 核心控制系統 (Control System)
* **主控板 (MCU)：** BigTreeTech Manta E3EZ。
* **核心運算 (SoC)：** BTT CB1。
* **韌體環境：** Klipper。
* **冷卻與散熱：** 風散對著鑽頭吹。

### 2. 運動與傳動架構 (Motion & Transmission)
* **軸向配置：** 雙 X 軸 (Dual X-Axis)、單 Y 軸 (Single Y-Axis)、單 Z 軸 (Single Z-Axis)。
* **傳動系統：** X、Y、Z 三軸皆採用 T8 螺桿 (T8 Lead Screw)。
* **步進馬達：** 42步進馬達。
* **歸零技術：** 採用 Sensorless Homing (無限位器歸零) 模式。

### 3. 主軸系統整合 (Spindle Integration)
* **驅動核心：** ZK-BM1 直流馬達驅動板。
* **控制模式：** 透過 Manta E3EZ 的 PWM 接口對接 ZK-BM1，實現轉速與啟停控制。
* **物理隔離：** 主軸驅動模組與主控板採物理分離，距離保持 15cm 以上。

### 4. 電氣與安全配置 (Power & Safety)
* **電源供應 (PSU)：** [請填寫電源供應器規格，例如：24V 350W]。
* **線材與佈線：** [請填寫線材規格，例如：是否使用拖鏈、屏蔽線]。
* **安全防護：** 實體緊急停止開關 (E-Stop) / 等電位接地。
