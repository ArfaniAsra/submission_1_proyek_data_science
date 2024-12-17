# Proyek Akhir: Menyelesaikan Permasalahan Human Resources

## Business Understanding

### Latar Belakang Bisnis
Jaya Jaya Maju adalah perusahaan multinasional yang telah berdiri sejak tahun 2000 dan memiliki lebih dari 1.000 karyawan yang tersebar di seluruh negeri. Walaupun telah berkembang pesat, perusahaan menghadapi tantangan signifikan dalam mengelola karyawan, terutama tingginya **attrition rate** atau tingkat keluar karyawan. Dengan angka attrition yang melebihi **10%**, perusahaan mulai merasakan dampak negatif seperti:
- **Biaya Rekrutmen Tinggi**: Berdasarkan karakteristik perusahaan yang memiliki lebih dari 1.000 karyawan, biaya yang dikeluarkan untuk proses rekrutmen dan pelatihan karyawan baru meningkat seiring tingginya angka pergantian karyawan. Hal ini mencakup biaya iklan lowongan kerja, seleksi, onboarding, dan pelatihan.
- **Penurunan Produktivitas**: Tingginya pergantian karyawan menyebabkan hilangnya pengalaman dan keterampilan yang dibutuhkan untuk mencapai target bisnis. Data dalam dataset seperti **YearsAtCompany** dan **YearsWithCurrManager** dapat membantu mengukur kontribusi pengalaman terhadap produktivitas.
- **Penurunan Kepuasan Karyawan**: Indikator kepuasan seperti **Job Satisfaction**, **Work-Life Balance**, dan **Environment Satisfaction** dalam dataset menunjukkan pentingnya mengidentifikasi ketidakpuasan lebih awal untuk mencegah gelombang keluar karyawan.

Manajemen HR di Jaya Jaya Maju menyadari pentingnya memahami faktor-faktor penyebab attrition agar dapat menyusun strategi yang tepat untuk **meningkatkan retensi karyawan** dan **mengurangi attrition rate** secara signifikan.

### Permasalahan Bisnis
Permasalahan bisnis yang akan diselesaikan melalui proyek ini adalah:
1. **Mengidentifikasi faktor-faktor utama yang mempengaruhi attrition rate** di perusahaan, baik dari segi demografis, kepuasan kerja, maupun metrik finansial.
2. **Mengukur tingkat kepuasan karyawan** berdasarkan parameter seperti **Job Satisfaction**, **Work-Life Balance**, dan **Environment Satisfaction**.
3. **Menentukan pola perilaku karyawan yang cenderung keluar**, seperti pengaruh jarak rumah ke kantor, lembur berlebihan (OverTime), dan pendapatan karyawan.
4. **Menyediakan alat bantu berupa business dashboard** yang memudahkan manajemen HR memantau dan menganalisis faktor-faktor penyebab attrition secara berkala.

Dengan menyelesaikan permasalahan ini, perusahaan diharapkan dapat:
- Mengurangi **attrition rate** dengan mengambil langkah pencegahan yang tepat.
- Menyusun program retensi yang lebih efektif.
- Meningkatkan kepuasan kerja dan produktivitas karyawan.

### Cakupan Proyek
Proyek ini mencakup:
1. **Eksplorasi dan Pemahaman Data**: Analisis dataset `employee_data.csv` untuk memahami karakteristik karyawan dan distribusi attrition.
2. **Data Preparation**: Membersihkan dan memproses data agar siap digunakan untuk analisis lebih lanjut.
3. **Analisis Faktor Penyebab Attrition**:
   - Analisis korelasi antara variabel seperti pendapatan, lembur, tingkat kepuasan, dan jarak rumah.
   - Visualisasi tren dan pola attrition di berbagai departemen, level pekerjaan, dan usia karyawan.
4. **Pembuatan Business Dashboard**: Visualisasi data dalam bentuk dashboard yang mudah dipahami untuk memantau faktor penyebab attrition.
5. **Kesimpulan dan Rekomendasi**: Menarik kesimpulan dari hasil analisis dan memberikan rekomendasi praktis untuk mengurangi attrition.

### Persiapan
- **Sumber Data**: Dataset `employee_data.csv` yang berisi informasi demografis, metrik kerja, dan flag attrition.
- **Setup Environment**:
```bash
pip install pandas numpy matplotlib seaborn
```

---

## Langkah Awal Eksplorasi Data

Kode berikut digunakan untuk memuat dataset, melihat ringkasan, dan melakukan eksplorasi awal:

```python
# Import library
import pandas as pd
import numpy as np

# Load dataset
df = pd.read_csv('employee_data.csv')

# Menampilkan ringkasan data
print("Informasi Dataset:")
print(df.info())

# Menampilkan preview data
print("\nPreview Data:")
print(df.head())

# Mengecek missing values
print("\nMissing Values:")
print(df.isnull().sum())

# Mengecek duplikat data
print("\nJumlah Duplikat:", df.duplicated().sum())
```

---

## Business Dashboard
Jelaskan tentang business dashboard yang telah dibuat. Jika ada, sertakan juga link untuk mengakses dashboard tersebut.

## Conclusion
Jelaskan konklusi dari proyek yang dikerjakan.

### Rekomendasi Action Items (Optional)
Berikan beberapa rekomendasi action items yang harus dilakukan perusahaan guna menyelesaikan permasalahan atau mencapai target mereka.

- action item 1
- action item 2
