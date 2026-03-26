# Fraud Risk Scoring System for Digital Banking

## Overview
Sistem machine learning untuk mendeteksi transaksi fraud dan menghasilkan **risk score (0–1)** sebagai dasar pengambilan keputusan secara real-time.

## Problem
- Kasus fraud (phishing, account takeover) terus meningkat  
- Data sangat imbalanced (<1% fraud)  
- Sistem tradisional masih rule-based dan kurang adaptif  

## Solution
- Model supervised ML untuk memprediksi probabilitas fraud  
- Menggunakan fitur perilaku (waktu, pola transaksi)  
- Output berupa risk score, bukan hanya label  

## Decision Rule
| Score | Action |
|------|--------|
| > 0.6 | Block |
| 0.3–0.6 | Verify (OTP) |
| < 0.3 | Allow |

## Key Insights
- Fraud cenderung punya skor lebih tinggi  
- Distribusi skor cukup terpisah jelas  
- Threshold sangat berpengaruh karena imbalance data  

## Tech Stack
Python, Pandas, Scikit-learn, Matplotlib  

## Dataset
https://www.kaggle.com/datasets/kartik2112/fraud-detection?resource=download  

## Notes
Dataset bersifat simulasi untuk keperluan pembelajaran.
