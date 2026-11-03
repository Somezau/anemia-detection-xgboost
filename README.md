# anemia-detection-xgboost
# Klasifikasi Anemia Menggunakan Algoritma XGBoost Berdasarkan Data Hematologi

## 1. Gambaran Umum Proyek

Proyek ini bertujuan untuk menganalisis kinerja algoritma Extreme Gradient Boosting (XGBoost) dalam melakukan klasifikasi anemia berdasarkan data hematologi.

Penelitian ini menggunakan beberapa skenario pembagian data latih dan data uji untuk membandingkan performa model dalam mengklasifikasikan kondisi anemia.

## 2. Tujuan Proyek

- Menerapkan algoritma XGBoost untuk klasifikasi anemia.
- Menguji kinerja model menggunakan beberapa skenario pembagian data.
- Membandingkan hasil klasifikasi berdasarkan metrik evaluasi.
- Menentukan skenario eksperimen dengan performa terbaik.

## 3. Dataset

Dataset yang digunakan merupakan data hematologi yang terdiri dari beberapa atribut pemeriksaan darah.

**Fitur yang digunakan:**
- Hemoglobin
- MCV (Mean Corpuscular Volume)
- MCH (Mean Corpuscular Hemoglobin)
- MCHC (Mean Corpuscular Hemoglobin Concentration)

**Variabel target:**
- `Result`: 0 = Tidak Anemia, 1 = Anemia.

Atribut Gender tidak digunakan dalam proses pemodelan.

## 4. Metodologi

Tahapan yang dilakukan dalam proyek ini meliputi:

1. Memuat dataset menggunakan Pandas.
2. Melakukan pemeriksaan dan preprocessing data.
3. Menentukan fitur yang digunakan dalam pemodelan.
4. Membagi dataset menjadi data latih dan data uji.
5. Melatih model menggunakan algoritma XGBoost.
6. Mengevaluasi hasil klasifikasi menggunakan metrik evaluasi.
7. Membandingkan performa model dari setiap skenario pengujian.

## 5. Skenario Eksperimen

Pengujian dilakukan menggunakan tiga skenario pembagian dataset:

| Skenario | Data Latih | Data Uji |
|---|---:|---:|
| 60:40 | 60% | 40% |
| 70:30 | 70% | 30% |
| 80:20 | 80% | 20% |

## 6. Hasil Evaluasi

Berdasarkan hasil pengujian, skenario pembagian data 70:30 dengan parameter `n_estimators = 100` menghasilkan performa terbaik.

| Metrik Evaluasi | Hasil |
|---|---:|
| Accuracy | 94,15% |
| F1-Score | 93,64% |

Hasil tersebut menunjukkan bahwa model mampu melakukan klasifikasi anemia dengan performa yang baik pada dataset yang digunakan.

## 7. Tools dan Teknologi

- Python
- Google Colab
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- XGBoost

## 8. Struktur Repository

```text
anemia-detection-xgboost/
│
├── README.md
├── .gitignore
├── Anemia_XGBoost_60_40.ipynb
├── Anemia_XGBoost_70-30.ipynb
├── Anemia_XGBoost_80-20.ipynb
├── Diagram_perbandingan_hasil.ipynb
└── anemia_dataset.csv
```

## 9. Kesimpulan

Proyek ini menunjukkan penerapan algoritma XGBoost dalam klasifikasi anemia berdasarkan data hematologi.

Melalui pengujian tiga skenario pembagian data, diperoleh bahwa skenario 70:30 menghasilkan performa terbaik berdasarkan nilai Accuracy dan F1-Score.

---

**Kategori:** Data Science | Machine Learning | Bioinformatics
