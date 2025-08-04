
# 🧠 Analisis Sentimen Ulasan Aplikasi ChatGPT di Google Play Store

Proyek ini bertujuan untuk menganalisis ribuan ulasan pengguna terhadap aplikasi ChatGPT di Google Play Store dan mengklasifikasikan sentimen mereka ke dalam tiga kategori: **positif**, **netral**, dan **negatif**.

## 📌 Tujuan
- Menggali persepsi publik terhadap aplikasi ChatGPT.
- Membangun model Machine Learning untuk klasifikasi sentimen.
- Mengevaluasi performa model terhadap data yang belum pernah dilihat.

## 📁 Dataset
Data dikumpulkan melalui web scraping dari halaman ulasan ChatGPT di Google Play Store menggunakan `google-play-scraper`, dan disimpan dalam file `ulasan_aplikasi_chatgpt.csv`.

## ⚙️ Teknologi & Tools
- Python
- Pandas, scikit-learn, matplotlib, wordcloud
- TF-IDF untuk ekstraksi fitur teks
- Algoritma: Random Forest, Naive Bayes, Logistic Regression, Decision Tree

## 🧪 Alur Analisis
1. **Scraping Data** ulasan dari PlayStore
2. **Preprocessing Teks** (lowercase, remove punctuation, stopwords)
3. **Label Sentimen** berdasarkan rating bintang:
   - 1-2 ⭐ = Negatif
   - 3 ⭐ = Netral
   - 4-5 ⭐ = Positif
4. **Ekstraksi Fitur** dengan TF-IDF
5. **Training Model** klasifikasi sentimen
6. **Evaluasi Performa** dengan classification report
7. **Visualisasi** dengan WordCloud per kelas sentimen

## 📊 Hasil
- Akurasi tertinggi dicapai oleh model **Random Forest** dan **Logistic Regression** dengan skor > 85%
- <img width="712" height="383" alt="Screenshot 2025-08-04 193552" src="https://github.com/user-attachments/assets/947b2410-d7cb-4e81-8b17-fcdfdae3b2cc" />
- Visualisasi WordCloud mengungkap kata-kata umum dari masing-masing sentimen
- Insight penting terkait kelebihan dan kekurangan aplikasi berdasarkan review publik


## 📷 Contoh Visualisasi
> WordCloud untuk Sentimen Positif, Netral, dan Negatif  
(*Tambahkan screenshot wordcloud di sini saat upload ke GitHub*)
<img width="859" height="547" alt="download" src="https://github.com/user-attachments/assets/752402b6-a3f9-49d5-8a04-171a50931153" />
<img width="859" height="547" alt="download" src="https://github.com/user-attachments/assets/a43228df-cc55-480e-9a0c-6a257d470e5e" />
<img width="1060" height="547" alt="download" src="https://github.com/user-attachments/assets/6f3936e0-274e-43ad-955f-e668bd60077e" />
### WordCloud
<img width="783" height="556" alt="download" src="https://github.com/user-attachments/assets/c083c37e-83ba-4e7a-a3e5-2a4b4d4cd89d" />
<img width="783" height="556" alt="download" src="https://github.com/user-attachments/assets/77e4a6c3-0a1c-4f2c-97d5-fef1f2455ab8" />
<img width="783" height="556" alt="download" src="https://github.com/user-attachments/assets/eccb7ca6-b6c5-4ec2-93e1-28a4e413b842" />

## 🚀 Cara Menjalankan Proyek
1. Clone repo ini
2. Install dependencies:
```bash
pip install -r requirements.txt
```
3. Jalankan notebook Jupyter `Analisis_Sentimen_Aplikasi_ChatGPT_pada_platform_PlayStore.ipynb`

## Insight
- Ulasan positif banyak berisi kata seperti: “membantu”, “cepat”, “mudah”
- Sentimen negatif cenderung muncul karena “error”, “berbayar”, atau “fitur terbatas”

## Kontribusi & Kontak
Proyek ini dibuat oleh [Pajar](https://github.com/pajarbeuy)  
Silakan hubungi saya untuk kolaborasi atau diskusi melalui [LinkedIn](https://www.linkedin.com/in/pajar-37421b296/)

---
