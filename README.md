# 🦠 Social Media Mining & Clustering: Tren Isu Flu A di TikTok

Sebuah eksplorasi data mining dan Social Network Analysis (SNA) terhadap ribuan data video publik TikTok terkait penyebaran Flu A/Influenza untuk memetakan dinamika respons masyarakat.

## 🎯 Tujuan Proyek
Melakukan ekstraksi data (scraping) otomatis, pembersihan teks, serta pengelompokan (*clustering*) topik darurat tanpa supervisi guna mengisolasi persebaran isu organik vs konten berita di media sosial.

## 🛠️ Tech Stack & Alat
* **Ekstraksi Data:** Apify TikTok Scraper
* **Pemrosesan Teks:** Python, Pandas, Regex, Sastrawi (Stopwords removal)
* **Topic Modelling & Clustering:** Scikit-Learn (TF-IDF Vectorization, K-Means Clustering, Latent Dirichlet Allocation / LDA)
* **Network Analysis:** NetworkX (Co-occurrence Hashtag Networks)
* **Visualisasi:** Matplotlib, Seaborn, WordCloud, PCA Scatter Plot

## 📈 Temuan & Hasil Utama
* **Skala Interaksi:** 261 sampel postingan merepresentasikan audiens masif dengan lebih dari **41.3 Juta Likes** dan **407 Juta Tayangan**.
* **Clustering Optimal (K-Means & LDA):** Evaluasi *Silhouette Score* menunjukkan **k=8** sebagai jumlah klaster terbaik, mengungkap bahwa narasi Flu A justru banyak didominasi dan bercampur dengan postingan akun agregator berita nasional.
* **Social Network Analysis (SNA):** Jaringan relasi terbangun dari **356 Node** (hashtag unik) dan **958 Edge**. Metrik *Degree Centrality* mengonfirmasi bahwa tagar `#influenza`, `#viral`, dan `#kesehatan` bertindak sebagai sentral/penghubung (*hub*) utama antar-komunitas topik.
