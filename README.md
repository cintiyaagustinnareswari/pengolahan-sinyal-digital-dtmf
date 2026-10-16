# Analisis dan Deteksi Nada DTMF pada Sinyal Audio Digital Menggunakan FFT

## 📌 Deskripsi Proyek

Proyek ini membahas implementasi dan analisis deteksi nada DTMF (*Dual-Tone Multi-Frequency*) dari sinyal audio hasil rekaman menggunakan *Fast Fourier Transform* (FFT).

DTMF merupakan sistem pensinyalan yang menggunakan kombinasi dua frekuensi untuk merepresentasikan tombol pada keypad telepon. Teknologi ini digunakan dalam sistem telepon, *Interactive Voice Response* (IVR), dan sistem kendali berbasis audio.

Sinyal DTMF dari rekaman nyata dapat mengandung noise, variasi amplitudo, serta jeda antar nada yang tidak seragam. Oleh karena itu, proyek ini menerapkan beberapa teknik pengolahan sinyal digital untuk membantu proses segmentasi dan identifikasi frekuensi DTMF.

## 🎯 Tujuan Proyek

1. Mengimplementasikan deteksi nada DTMF dari sinyal audio hasil rekaman.
2. Menganalisis pengaruh filter FIR terhadap kualitas sinyal.
3. Mengevaluasi pengaruh variasi threshold terhadap proses segmentasi nada.
4. Membandingkan penggunaan *window function* dalam analisis spektrum frekuensi.
5. Mengidentifikasi pasangan frekuensi yang merepresentasikan digit pada keypad telepon.

## 🔬 Metode yang Digunakan

### 1. Bandpass Filter FIR

Filter FIR (*Finite Impulse Response*) digunakan untuk membatasi frekuensi sinyal pada rentang yang relevan dengan frekuensi standar DTMF. Tahap ini bertujuan mengurangi komponen frekuensi di luar rentang yang diperlukan.

### 2. Segmentasi Sinyal

Segmentasi dilakukan menggunakan envelope dan threshold untuk memisahkan bagian sinyal yang mengandung nada DTMF dari bagian jeda atau keheningan.

### 3. Fast Fourier Transform (FFT)

FFT digunakan untuk menganalisis spektrum frekuensi pada setiap segmen sinyal. Hasil analisis digunakan untuk mengidentifikasi komponen frekuensi rendah dan tinggi yang membentuk nada DTMF.

### 4. Perbandingan Window Function

Beberapa *window function*, seperti Rectangular, Hamming, dan Hann, dibandingkan untuk mengamati pengaruhnya terhadap spektrum frekuensi dan proses identifikasi nada.

### 5. Evaluasi Threshold

Variasi nilai threshold dianalisis untuk mengetahui pengaruhnya terhadap jumlah segmen yang terdeteksi dan kejelasan pemisahan antar nada.

## 📊 Hasil yang Diharapkan

- Visualisasi sinyal audio dalam domain waktu.
- Visualisasi spektrum frekuensi menggunakan FFT.
- Segmentasi nada DTMF berdasarkan envelope dan threshold.
- Identifikasi pasangan frekuensi sesuai standar keypad telepon.
- Perbandingan hasil analisis berdasarkan variasi threshold dan *window function*.

## 🛠️ Teknologi yang Digunakan

- Python
- NumPy
- SciPy
- Matplotlib
- Jupyter Notebook

*Daftar teknologi dapat disesuaikan dengan library yang benar-benar digunakan dalam proyek.*

## 📁 Struktur Repository

```text
Pengolahan-Sinyal-Digital/
├── Dataset/
│   └── audio_dtmf
├── Notebook/
│   └── analisis_dtmf.ipynb
├── Output/
│   └── visualisasi/
└── README.md
```

Struktur tersebut merupakan contoh dan dapat disesuaikan dengan susunan file yang sebenarnya di repository.

## 🎓 Tugas Akademik

Proyek ini dikembangkan sebagai bagian dari pemenuhan tugas akademik pada mata kuliah **Pengolahan Sinyal Digital**.

Melalui proyek ini, mahasiswa menerapkan konsep pengolahan sinyal digital, meliputi *filtering*, segmentasi sinyal, analisis spektrum frekuensi menggunakan Fast Fourier Transform (FFT), serta deteksi nada DTMF dari sinyal audio hasil rekaman.

Proyek ini juga bertujuan untuk memperdalam pemahaman mengenai penerapan transformasi Fourier dan teknik pemrosesan sinyal dalam mengidentifikasi frekuensi pada sistem pensinyalan telepon.

### Informasi Akademik

- **Jenis Proyek:** Tugas Akademik
- **Mata Kuliah:** Pengolahan Sinyal Digital
- **Topik:** Analisis dan Deteksi Nada DTMF
- **Metode Utama:** Fast Fourier Transform (FFT)

## 📝 Kesimpulan

Proyek ini menerapkan teknik pengolahan sinyal digital untuk menganalisis dan mengidentifikasi nada DTMF pada sinyal audio. Penggunaan filter FIR, segmentasi berbasis threshold, FFT, dan *window function* menjadi bagian dari proses analisis untuk memahami karakteristik frekuensi setiap nada.

Evaluasi terhadap variasi threshold dan *window function* dapat membantu memahami faktor-faktor yang memengaruhi proses deteksi. Hasil akhir dan tingkat keberhasilan sistem ditentukan berdasarkan implementasi serta pengujian yang dilakukan pada notebook proyek.

---

*Repository ini dibuat untuk keperluan tugas akademik dan pembelajaran Pengolahan Sinyal Digital.*
