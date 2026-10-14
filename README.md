# 🌿 GreenPulse: Smart Irrigation Decision Support System

<p align="center">
  <b>Sistem pendukung keputusan penyiraman tanaman berbasis Machine Learning & data sensor lingkungan untuk pertanian skala mikro / rumah tangga</b>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Status-Completed-success" alt="Status">
  <img src="https://img.shields.io/badge/Python-3.10%2B-blue" alt="Python">
  <img src="https://img.shields.io/badge/FastAPI-Backend-teal" alt="FastAPI">
  <img src="https://img.shields.io/badge/Scikit--Learn-Machine%20Learning-orange" alt="Scikit-Learn">
  <img src="https://img.shields.io/badge/Deployed-Vercel-black" alt="Vercel">
</p>

<p align="center">
  <a href="https://smart-irrigation-web-ai-xt1z.vercel.app"><b>🚀 Buka Live Demo</b></a>
</p>

---

## 🚀 Live Demo
Coba langsung aplikasi GreenPulse di sini:

👉 **[smart-irrigation-web-ai-xt1z.vercel.app](https://smart-irrigation-web-ai-xt1z.vercel.app)**

---

## 📌 Overview
**GreenPulse** adalah sistem pendukung keputusan (*decision support system*) berbasis AI untuk membantu perawatan tanaman pot *indoor* secara efisien dan berbasis data.

Masalah yang diselesaikan: penyiraman yang tidak konsisten sering menyebabkan stres fisiologis hingga kematian tanaman akibat *underwatering* maupun *overwatering*. GreenPulse memprediksi kebutuhan air tanaman dari kondisi lingkungan mikro, yaitu **kelembaban tanah**, **suhu tanah**, dan **kelembaban udara**.

---

## ✨ Key Features
- **AI-Driven Prediction:** Model *Logistic Regression* mengklasifikasikan kondisi tanaman menjadi *Healthy* atau *Needs Watering*.
- **Hybrid Decision System:** Probabilitas dari AI dipadukan dengan batas pengaman agronomis (*rule-based threshold*, kelembaban tanah < 35%) agar keputusan tetap aman bagi tanaman.
- **Interactive Dashboard:** Pantau status tanaman, lihat grafik historis kelembaban, serta kelola daftar tanaman (*Add Plant* & *Pick Plant*).
- **Monitoring & History Logging:** Riwayat input sensor dan keputusan AI tercatat per tanaman, lengkap dengan penandaan aktivitas penyiraman.
- **Simulasi & Kontrol:** Halaman simulasi untuk mengatur parameter sensor dan mencoba skenario berbeda.

---

## 🛠️ Tech Stack
| Layer | Teknologi |
|---|---|
| Language | Python |
| Machine Learning | Scikit-Learn, Pandas, NumPy, Joblib |
| Backend API | FastAPI, Uvicorn, SQLAlchemy |
| Frontend | HTML, CSS, JavaScript (Responsive Dashboard) |
| Deployment | Vercel |
| Dataset | Mendeley Data, *Environmental Sensor Monitoring Dataset* |

---

## 📊 Machine Learning Pipeline
1. **Preprocessing & Normalization:** `StandardScaler` di dalam scikit-learn `Pipeline` agar skala data konsisten antara training dan production.
2. **Model Evaluation:** Diuji dengan *Stratified K-Fold Cross-Validation*, menghasilkan *Balanced Accuracy* mendekati `0.999`.
3. **Feature Importance:** Analisis koefisien menunjukkan *Soil Moisture* adalah faktor paling dominan, didukung suhu dan kelembaban udara sebagai variabel kontekstual.

---

## 👥 Team
Proyek kolaboratif mahasiswa Computer Science, BINUS University Malang:

| Nama | NIM | Peran |
|---|---|---|
| Jesselyn Angelia Luwuk | 2802420252 | Lead Researcher, AI Modeler |
| Maria Yohana Vianny Leo | 2802538813 | Data Analyst, ML Engineer, Full-Stack Developer |
| Faisal Ramdhani | 2802444302 | UI/UX Designer |
---
