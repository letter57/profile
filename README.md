
# 履歷（Firmware / Embedded System Engineer）

## 基本資料

姓名：陳威達 (Cris Chen)  

職稱：Firmware / Embedded System Engineer

經驗：19 年

地點：台中

---

## 專業摘要（Summary）

具備跨領域整合能力的嵌入式系統工程師，專長於 **RTOS（Zephyr / FreeRTOS）、BLE / Zigbee 應用、RFID系統整合**，同時具備電路設計、PCB Layout 與 3D 結構設計能力，能獨立完成產品從概念、設計到實作與量產前打樣。

曾自主開發整合 **RFID 多UID切換 + BLE HID 遙控功能產品**，具備完整產品化經驗（硬體 / 韌體 / 機構 / 使用者體驗設計）。

---

## 核心技能（Core Skills）

### Embedded / Firmware

* C / Embedded C
* RTOS：Zephyr OS、FreeRTOS
* LVGL GUI Development
* BLE HID（鍵盤 / 遙控應用）
* Zigbee (doorlock應用)
* NFC / RFID（UID複製、多卡模擬）
* Peripheral：UART / I2C / SPI / ADC / GPIO / PWM / RS485

### Hardware Design

* 電路設計（Schematic）
* PCB Layout（Altium Designer / KiCad）
* 低功耗設計（CR2032 應用）

### System Integration

* BLE + RFID 整合應用
* 低功耗裝置設計
* 使用者操作流程（UX：按鍵 / LED）
* 量測分析
* DFU

### Mechanical / Prototyping

* SolidWorks / FreeCAD
* 3D Printing（產品外殼開發與打樣）

### Tools

* Git（版本控制）
* VS Code / Embedded Toolchains

---

## 專案經驗（Projects）

### 🔐 智慧門鎖系統開發（Smart Door Lock System）

**角色：系統架構設計 / 韌體 / 硬體**

**專案描述：**
負責智慧門鎖產品之嵌入式系統開發與整合，涵蓋身分辨識、無線通訊、人機介面與電源管理等核心功能，打造具備多通訊能力與高可靠度的 IoT 門禁解決方案，產品支援人臉辨識、RFID 卡片、密碼、BLE App 等多元解鎖方式。

**技術重點：**

* 嵌入式系統整合
  * 負責整體系統架構設計與模組整合（RFID、BLE、Zigbee、HMI）
  * 韌體開發與跨模組協調（輸入 / 輸出 / 通訊）
* RFID 身分辨識
  * 建立使用者驗證流程與UID管理機制.
  * 整合記憶體儲存（EEPROM / Flash）以管理使用者資料.
* 無線通訊（BLE / Zigbee）
  * 實作門鎖與行動裝置 / IoT系統之無線連線.
  * 處理配對、資料傳輸與連線穩定性問題.
* 人機介面（HMI）設計
  * 電容式觸控按鍵（Capacitive Touch）調校與抗雜訊優化.
  * 整合 LED 指示燈、語音 IC、蜂鳴器，提升操作回饋體驗.
* 機構控制與驅動
  * 馬達驅動（Motor Driver）控制門鎖開關動作.
  * 設計安全機制（異常保護 / 狀態判斷）.
* 電源管理
  * 電池電量偵測（ADC）與電壓換算.
  * 低電量警示與系統保護機制.
* 時間與資料管理
  * 整合 RTC（Real-Time Clock）實現時間紀錄功能.
  * 儲存與管理開鎖紀錄與使用者資訊.
* 系統測試與除錯
  * 使用示波器 / 邏輯分析儀進行訊號分析與問題排除.
  * 提升系統穩定度與量產品質.

**MCU / Platform Experience：**
* Nordic Semiconductor（nRF52)
  * 使用 nRF52 系列開發 BLE 裝置（Zephyr RTOS）
  * 使用 nRF52 系列開發 智慧門鎖功能（Zephyr RTOS）
  * 熟悉低功耗設計（Sleep / Advertising Optimization）
  * 使用 nRF Connect SDK 進行開發與除錯
* Microchip (PIC18)
  * 使用 PIC MCU 進行嵌入式系統開發
  * 周邊控制（UART / I2C / SPI / ADC）
  * 應用於門鎖控制系統（RFID / Motor Driver / Keypad）
* NXP (i.MX RT1060）
  * 人臉辨識整合
  * Camera 資料擷取與影像處理 pipeline.
  * 使用 LVGL 建立 UI（畫面顯示 / 狀態回饋 / 操作流程）
  * MCU 資源分配與效能優化（RAM / Flash / FPS）
  * RTOS 任務整合（影像處理 + UI 顯示）

**成果：**

* 成功完成多模組（RFID / BLE / Zigbee）整合，打造具備多通訊能力之智慧門鎖系統.
* 提升電容觸控按鍵穩定性，降低誤觸與環境干擾影響.
* 建立完整電源管理機制，有效提升電池使用壽命.
* 完成系統整合與量產導入，提升產品可靠度與市場競爭力.

**Product Reference：**
* [WAFERLOCK L600 Product Page](https://www.waferlock.com/tw/product/L600?utm_source=chatgpt.com)
* [WAFERLOCK L600 Demonstration Video](https://www.youtube.com/watch?v=5aBnQ_c86Zk)

---
### 🔹 RFID 多UID切換 + BLE HID 一鍵拍照裝置（個人專案）

**角色：系統架構設計 / 韌體 / 硬體 / 機構（全包）**

**專案描述：**
開發一款整合 RFID 複製卡與 BLE HID 功能的隨身裝置，可支援多組 UID 切換與手機遠端拍照控制，提升日常門禁與拍照體驗。

**技術重點：**

* 使用 Zephyr OS 開發 BLE HID（模擬鍵盤拍照）
* RFID UID 多組切換設計（按鍵 + LED 狀態提示）
* 低功耗設計（CR2032 電池供電）
* PCB 設計與 Layout（KiCad）
* 3D 外殼設計與列印（產品化打樣）

**MCU / Platform Experience：**

* Nordic Semiconductor（nRF52）
  * 使用 nRF52 系列開發 BLE 裝置（Zephyr RTOS）
  * 實作 BLE HID（鍵盤 / 遙控拍照）
  * 熟悉低功耗設計（Sleep / Advertising Optimization）
  * 使用 nRF Connect SDK 進行開發與除錯

**成果：**

* 成功整合 RFID 與 BLE 雙功能於單一裝置
* 建立完整產品開發流程（硬體→韌體→外殼）
* 已應用於實際銷售與市場測試

---

## 工作經驗（Work Experience）

### 維夫拉克｜Firmware Engineer

期間：2011 / 4 – Present

**工作內容：**

* 嵌入式系統開發（MCU 韌體設計）
* RTOS 系統開發與維護
* 硬體電路設計與除錯
* 周邊介面整合（I2C / SPI / UART / ADC / PWM / RS485）

**成果（請補數據）：**

* 提升系統穩定度 XX%
* 降低功耗 XX%
* 專案如期交付（XX 個專案）

---
### 協記精密工業股份有限公司｜Electrical Engineer

期間：2007 / 3 – 2011 / 4

**工作內容：**

* 硬體設計
* PCB Layout
* 韌體開發
* 量產導入
* 家電產品
  * 釘槍
  * 電熱毯
  * 馬達緩啟動
  * 吊扇發射器
 * 運動器材
   * 跑步機控制面板
 * 治具
   * 50Hz/60Hz 波形產生器

---

## 加分項目（Additional）

* 具備完整產品開發能力（Firmware + Hardware + Mechanical）
* 熟悉 IoT / BLE 應用場景
* 具備商品化與市場導向思維（蝦皮產品實作）

---

## 作品集（Portfolio）
* [RFID Multi-UID Switchable CARD + BLE HID Remote Shutter](https://github.com/letter57/WFEGO_000007/blob/master/Personal_Project/Personal_Project.md)   
* [ReflowSoldering](https://github.com/letter57/ReflowSoldering)
* [1.3 吋 顯示模組與客製化外殼開發](https://github.com/letter57/WFEGO_000004)
* [Zephyr RTOS 跨平台移植與驗證實作](https://github.com/letter57/zephyr-cross-platform-demo)
