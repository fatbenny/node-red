# 台灣環境資訊 Dashboard

本專案為一個整合台灣環境即時資料的 Dashboard，包含空氣品質、天氣資訊及即時影像監視器畫面，提供一站式的環境觀測平台。

## 功能特色

- 🌫️ 即時取得 **環保署空氣品質** 資訊（AQI、PM2.5、PM10 等）
- ☀️ 即時取得 **氣象局天氣資訊**（溫度、降雨機率、濕度等）
- 🎥 整合來自 **台灣即時影像監視器** 的即時畫面
- 📊 以 **Dashboard 介面** 呈現所有資訊，支援圖表與地圖視覺化

## 資料來源

- [行政院環保署空氣品質監測網](https://data.moenv.gov.tw/api/v2/AQX_P_432?api_key=*****)
- [中央氣象署開放資料平台](https://opendata.cwa.gov.tw/api/v1/rest/datastore/O-A0001-001?Authorization=*****)
- [交通部即時影像監視器](https://hls.bote.gov.taipei/live/index.html?id=${this.camId})

## 系統架構

```mermaid
graph TD
  A[環保署 API] --> D[Dashboard]
  B[氣象局 API] --> D
  C[即時影像資料] --> D
