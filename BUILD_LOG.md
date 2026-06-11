# DIY CNC — 建構日誌

> 專案：將舊款 3D 列印機改造為 CNC 銑床  
> 主控：BigTreeTech Manta E3EZ + CB1 | 韌體：Klipper

---

## Phase 1 — 機架組裝

**說明：**  
（補充：改造來源機型、鋁擠型規格、鎖件選用等）

**完成內容：**
- 黑色鋼板框架組立
- T8 螺桿 + 光軸線性滑軌安裝
- 銅螺母座定位

**機架正面**  
![機架正面](images/phase1_01_frame_front.jpg)

**機架斜角**  
![機架斜角](images/phase1_03_frame_angle.jpg)

**機架含輪子**  
![機架含輪子](images/phase1_04_frame_wheels.jpg)

**機架後方**  
![機架後方](images/phase1_05_frame_rear.jpg)

**螺桿側視**  
![螺桿側視](images/phase1_02_leadscrew_side.jpg)

**螺桿銅螺母**  
![螺桿銅螺母](images/phase1_06_leadscrew_nut.jpg)

**螺桿聯軸器**  
![螺桿聯軸器](images/phase1_07_leadscrew_coupler.jpg)

---

## Phase 2 — 運動系統安裝

**說明：**  
（補充：雙X軸設計原因、Z軸行程、步進馬達型號等）

**完成內容：**
- X / Y / Z 軸螺桿與滑塊安裝
- 42 步進馬達與聯軸器組裝
- 主軸座（3D 列印件）安裝
- 鋁擠型強化側柱鎖固

**組裝中**  
![組裝中](images/phase2_01_assembly.jpg)

**Z 軸座安裝**  
![Z軸座安裝](images/phase2_02_z_axis_mount.jpg)

**主軸支架特寫**  
![主軸支架特寫](images/phase2_03_spindle_bracket.jpg)

**框架俯視**  
![框架俯視](images/phase2_04_frame_topdown.jpg)

**X 軸導軌**  
![X軸導軌](images/phase2_05_x_rails.jpg)

**3D 列印滑車**  
![3D列印滑車](images/phase2_06_printed_carriage.jpg)

**Y 軸**  
![Y軸](images/phase2_07_y_axis.jpg)

**Z 軸安裝過程**  
![Z軸安裝過程](images/phase2_08_z_install.jpg)

---

## Phase 3 — 電控系統

**說明：**  
（補充：接線過程遇到的問題、EMI 處理方式等）

**完成內容：**
- BTT Manta E3EZ + CB1 主機板安裝
- Mean Well NES-350-24 電源供應器接線
- 步進馬達驅動器插裝
- 主電源開關 + 緊急停止接線

| 元件 | 型號 |
|------|------|
| 主控板 | BTT Manta E3EZ |
| 運算核心 | BTT CB1 (H616) |
| 電源 | Mean Well NES-350-24 |
| 驅動器 | （補充型號） |

**電控底板**  
![電控底板](images/phase3_01_electronics_tray.jpg)

**主機板特寫**  
![主機板特寫](images/phase3_02_board_closeup.jpg)

**BTT Manta E3EZ**  
![BTT Manta E3EZ](images/phase3_03_manta_e3ez.jpg)

**電控面板整體**  
![電控面板整體](images/phase3_04_electronics_panel.jpg)

---

## Phase 4 — 整機整合

**說明：**  
（補充：壓克力護板製作方式、螢幕固定方案等）

**完成內容：**
- BTT TFT35 觸控螢幕安裝
- 壓克力側板封裝
- 走線整理與固定
- DC 主軸馬達安裝（ZK-BM1 驅動）

**電控上機**  
![電控上機](images/phase4_01_machine_electronics.jpg)

**側面走線**  
![側面走線](images/phase4_02_side_wiring.jpg)

**主軸馬達**  
![主軸馬達](images/phase4_03_spindle_motor.jpg)

**機架早期狀態**  
![機架早期狀態](images/phase4_04_frame_early.jpg)

**框架（地面施工）**  
![框架地面施工](images/phase4_05_frame_concrete.jpg)

**夜間施工**  
![夜間施工](images/phase4_06_machine_bedroom.jpg)

**整機直立**  
![整機直立](images/phase4_07_machine_upright.jpg)

**聯軸器特寫**  
![聯軸器特寫](images/phase4_08_coupling_closeup.jpg)

**軸承座**  
![軸承座](images/phase4_09_bearing_block.jpg)

**DC 主軸**  
![DC主軸](images/phase4_10_dc_spindle.jpg)

**四軸步進馬達**  
![四軸步進馬達](images/phase4_11_four_steppers.jpg)

**TFT 螢幕安裝**  
![TFT螢幕安裝](images/phase4_12_tft_screen.jpg)

**木質加工床**  
![木質加工床](images/phase4_13_machine_wood_bed.jpg)

**壓克力側板**  
![壓克力側板](images/phase4_14_acrylic_panels.jpg)

**整機正面**  
![整機正面](images/phase4_15_front_view.jpg)

**整機斜角**  
![整機斜角](images/phase4_16_angle_view.jpg)

---

## Phase 5 — 首次試切

**說明：**  
（補充：使用軟體、G-code 來源、切削參數等）

**完成內容：**
- Klipper 韌體設定完成
- 歸零測試通過
- 首次切削：木板輪廓切割 + 笑臉雕刻

| 參數 | 數值 |
|------|------|
| 材料 | 薄木板 |
| 主軸轉速 | （補充） |
| 進給速度 | （補充） |
| 切削深度 | （補充） |

**切削中**  
![切削中](images/phase5_01_cutting_in_progress.jpg)

**龍門架正面**  
![龍門架正面](images/phase5_02_gantry_front.jpg)

**整機含護板**  
![整機含護板](images/phase5_03_machine_panels.jpg)

**X 軸俯視**  
![X軸俯視](images/phase5_04_x_axis_top.jpg)

**實驗室中運作**  
![實驗室中運作](images/phase5_05_lab_view.jpg)

**整機側面**  
![整機側面](images/phase5_09_machine_side.jpg)

**整機正面（完成）**  
![整機正面完成](images/phase5_10_machine_front_clean.jpg)

**龍門架俯視**  
![龍門架俯視](images/phase5_11_gantry_above.jpg)

**底部視角**  
![底部視角](images/phase5_13_machine_bottom.jpg)

**首切成果 1**  
![首切成果1](images/phase5_06_first_cut1.jpg)

**首切成果 2**  
![首切成果2](images/phase5_07_first_cut2.jpg)

**首切成果 3**  
![首切成果3](images/phase5_08_first_cut3.jpg)

**首切成果 4**  
![首切成果4](images/phase5_14_first_cut4.jpg)

**首切成果 5**  
![首切成果5](images/phase5_15_first_cut5.jpg)

**首切成果 6**  
![首切成果6](images/phase5_16_first_cut6.jpg)

---

## 問題紀錄

| 日期 | 問題描述 | 解決方式 |
|------|----------|----------|
| | | |

---

## 待辦 / 後續改進

- [ ] （補充）
- [ ] （補充）
