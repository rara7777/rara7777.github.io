# AWS Snow Family 簡介與歷史演進

AWS Snow Family 是一系列針對**大量資料遷移**與**邊緣運算（Edge Computing）**需求所設計的裝置與服務，特別適用於以下場景：

- 網路頻寬受限的環境
- 需要在本地進行資料處理的應用
- 大量資料需要快速且安全地遷移至 AWS 的情況

---

## ❄️ Snowcone（已終止服務）

> 📆 終止時間：2024 年 11 月 12 日
>
- 提供 **8 TB** 儲存容量
- 小巧輕便，具備防摔、防震、防塵、防水與耐極端溫差的特性
- 適用於本地端的**儲存、資料處理與傳輸**
- 支援兩種資料上傳方式：
    - 使用 **AWS DataSync**，透過網路傳輸資料至 AWS
    - 將裝置寄回 AWS，由 AWS 協助上傳
- 可透過 **AWS OpsHub** 管理與設定 Snow Family 裝置
- 影片資源：
    - [Snowcone 介紹影片](https://youtu.be/R-yfD-aROKM)
    - [Snowcone 案例 - 野外影音轉碼](https://youtu.be/X_8LM7E_hiE?feature=shared)

---

## 📦 Snowball（現為唯一仍提供的 Snow Family 成員）

Snowball 是一種用於**大規模資料遷移與邊緣運算**的裝置，提供兩種型號：

- **Snowball Edge Storage Optimized**
    - 高容量儲存，最高達 **210 TB NVMe**
    - 支援每秒高達 **1.5 GB** 的資料傳輸速度
- **Snowball Edge Compute Optimized**
    - 強化運算資源，最多 **104 vCPUs**
    - 配備 **全 SSD，28 TB NVMe 儲存空間**，適合需要在邊緣執行分析或機器學習任務的場景

### 功能特色：

- 可雙向傳輸資料（從 AWS 傳出或傳入）
- 適用於資料中心搬遷、大量影片素材搬移、離線資料備份等情境
- 影片資源：
    - [大規模資料遷移案例影片](https://youtu.be/9uc2DSZ1wL8?feature=shared)

---

## 🚛 Snowmobile（已終止服務）

> 📆 終止時間：2024 年 4 月
>
- 提供 **高達 100 PB** 的容量
- 本質是一台裝載多個 Snowball 的大型卡車
- 搭載：
    - **溫控系統、GPS 定位、24 小時監控攝影機**
    - 可選配 **保全人員護送**
- 適用於超過 10 PB 的極大資料搬移場景

### 停止服務原因：

- 高昂的人力與硬體維運成本（如駕駛、停車、電力與冷卻）
- 使用率偏低，因多數企業只需 Snowball 就能完成遷移任務
- 隨著網路傳輸技術進步，多數資料搬移不再需要如此大型的實體設備
- 影片資源：
    - [Snowmobile 展示影片](https://youtu.be/8vQmTZTq7nw?feature=shared)

---

## 🧠 使用時的評估原則

在選擇 Snow Family 之前，請評估以下幾點：

1. **資料總量**：您的資料量有多大？
2. **現有網路頻寬與穩定性**：透過現有網路上傳資料至 S3 需要多少時間？
3. **時間成本 vs 裝置寄送成本**：哪種方式更快、更穩定、總成本更低？

---

## 📉 現況與總結（截至 2025 年）

- 2024 年 AWS 宣布終止 **Snowcone** 與 **Snowmobile**，目前僅剩 **Snowball Edge** 系列仍在提供服務
- 停止原因與時代背景有關：
    - 現今企業環境中，**網路頻寬大幅提升**
    - 搭配 AWS 的其他工具（如 **DataSync**、**Direct Connect**、**Outposts**），資料傳輸變得更簡單與高效

---

## 📚 延伸閱讀與參考資源

- [AWS 官方部落格：Snow Family 裝置更新](https://aws.amazon.com/tw/blogs/storage/aws-snow-device-updates/)
- [Snowcone 官方介紹](https://www.aboutamazon.com/news/aws/introducing-aws-snowcone-a-small-ultra-portable-edge-computing-and-data-transfer-device)
- [Searce Blog：Meet the AWS Snow Family](https://blog.searce.com/meet-the-aws-snow-family-your-coolest-allies-in-the-cloud-18dd041d7b42)
- [Snowcone 案例影片](https://youtu.be/X_8LM7E_hiE)
- [Snow Family 整體介紹影片](https://youtu.be/SFmT6hf4m4g)
