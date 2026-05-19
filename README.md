# COVMAP Indonesia (Covid-19 Mapping Indonesia) 🇮🇩🦠

![Timeline](https://img.shields.io/badge/Timeline-Sep_2023-8A2BE2)
![Dataset](https://img.shields.io/badge/Dataset-Kaggle-blue?logo=kaggle)
![Tools](https://img.shields.io/badge/Visualization-Looker_Studio-orange)
![Status](https://img.shields.io/badge/Status-Completed-success)

**COVMAP Indonesia** adalah sebuah proyek analisis data dan visualisasi yang menyajikan peta interaktif persebaran COVID-19 di Indonesia. Proyek ini bertujuan untuk mengubah data mentah menjadi wawasan (*insights*) yang jelas dan informatif mengenai dampak pandemi dari tahun 2020 hingga 2022.

> **Waktu Pengerjaan:** September 2023

---

## 🔗 Tautan Dashboard
**[Klik di sini untuk melihat Dashboard COVMAP Indonesia secara interaktif di Looker Studio]((https://lookerstudio.google.com/reporting/5f7d260d-a6c9-4714-98e1-e560fa8a5748))**

<!-- Silakan unggah screenshot dashboard Anda ke GitHub, lalu ganti tautan di bawah -->
![Preview Dashboard COVMAP](https://via.placeholder.com/800x400?text=Screenshot+Dashboard+Looker+Studio)

---

## ✨ Fitur Utama Analisis

1. **Peta Interaktif Persebaran (Mapping)** 🗺️

   Menyajikan peta interaktif yang memvisualisasikan persebaran COVID-19 di seluruh provinsi di Indonesia secara jelas dan informatif.

3. **Akumulasi Kasus (2020 - 2022)** 📈

   Menampilkan total kasus terkonfirmasi dari tahun 2020 hingga akhir tahun 2022 dalam format angka dan metrik yang komprehensif.

4. **Metrik Kematian (Fatality Analysis)** ⚰️

   Menyediakan data yang mendetail dan akurat mengenai angka kematian (*mortality rate*) yang disebabkan oleh virus COVID-19.

5. **Identifikasi Titik Kritis (Hotspots)** 🔴

   Menyoroti provinsi-provinsi dengan angka kasus positif dan tingkat kematian tertinggi untuk membantu memahami pola persebaran virus dengan cepat.

7. **Tinjauan Tren Waktu (Time-Series Trend)** ⏳

   Menyajikan grafik tren pandemi dari waktu ke waktu (berdasarkan bulan/tahun) sebagai bahan evaluasi historis dan pembelajaran penanganan wabah.

---

## 🛠️ Alat & Sumber Data

* **Sumber Data:** [Kaggle](https://www.kaggle.com/datasets/hendratno/covid19-indonesia) (Dataset COVID-19 Indonesia)
* **Visualisasi & BI Tool:** Google Looker Studio
* **Pengolahan Data:** Python

---

## 🔄 Alur Pemrosesan Data (Data Pipeline)

```mermaid
graph LR
    A[(Dataset Kaggle)] -->|Unduh & Ekstrak| B(Pengolahan/Pembersihan Data (Python))
    B -->|Import Data| C[Google Looker Studio]
    C -->|Visualisasi Data| D{Dashboard COVMAP}
    
    style A fill:#20beff,stroke:#fff,stroke-width:2px,color:#fff
    style C fill:#ff8c00,stroke:#fff,stroke-width:2px,color:#fff
