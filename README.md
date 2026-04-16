# 🚕 Taxi Trip Analysis

## 📌 Deskripsi Proyek
Industri ride-hailing memiliki nilai pasar yang sangat besar, mencapai sekitar USD 163.55 miliar pada tahun 2025. Namun, kenaikan harga perjalanan terbukti dapat menurunkan penggunaan layanan, sehingga strategi pricing menjadi faktor krusial dalam menentukan revenue.

Proyek ini bertujuan untuk menganalisis faktor-faktor yang memengaruhi harga perjalanan (Trip Price) dan kontribusinya terhadap revenue, sehingga dapat membantu perusahaan dalam mengoptimalkan strategi pricing berbasis data.

---

## 🎯 Tujuan Analisis
- Mengidentifikasi faktor utama yang memengaruhi Trip Price  
- Menganalisis pengaruh variabel operasional dan eksternal (waktu, lalu lintas, cuaca)  
- Mengidentifikasi segmen perjalanan dengan kontribusi revenue terbesar  
- Memberikan rekomendasi strategis untuk optimalisasi pricing  

---

## 📂 Dataset
- Sumber: Kaggle (Taxi Trip Price Dataset)  
- Jumlah data: 1000 baris  

**Fitur utama:**
- Trip Distance (km)  
- Trip Duration (minutes)  
- Passenger Count  
- Traffic Conditions  
- Weather  
- Base Fare, Per Km Rate, Per Minute Rate  
- Trip Price  

---

## ⚙️ Proses Analisis

### 1. Data Cleaning
- Menangani 549 missing value menggunakan:
  - Kategori → “Unknown”  
  - Numerik → mean & median  
- Tidak ditemukan data duplikat  

### 2. Handling Outlier
- Outlier ditemukan pada Trip Distance dan Trip Price  
- Outlier tetap dipertahankan karena mencerminkan kondisi nyata  

### 3. Feature Engineering
- Speed (km/h)  
- Price per Km  
- Price per Minute  
- Distance Category & Speed Category  

### 4. Exploratory Data Analysis (EDA)
- Analisis distribusi data  
- Analisis korelasi antar variabel  
- Visualisasi hubungan antara faktor operasional dan harga  

---

## 📊 Key Insights

### 1. Jarak perjalanan adalah faktor utama penentu harga
- Korelasi kuat antara jarak dan harga (0.83)  
- Semakin jauh perjalanan, semakin tinggi harga  
- Durasi dan jumlah penumpang tidak signifikan  

### 2. Faktor eksternal memengaruhi harga perjalanan
- Lalu lintas padat → harga lebih tinggi (~$64)  
- Waktu siang–malam → harga lebih tinggi (~$56–$60)  
- Menunjukkan adanya pengaruh demand terhadap harga  

### 3. Segmen jarak jauh mendominasi revenue
- Long distance: ~45% revenue ($25.47K)  
- Medium: ~28%  
- Very short: hanya ~3.8%  

### 4. Weekday menghasilkan revenue lebih tinggi
- Weekday: ~$37.74K  
- Weekend: ~$16.17K  

---

## 💡 Business Recommendations

### 1. Optimalkan pricing berbasis jarak
- Fokus pada distance sebagai driver utama pricing  
- Jadikan jarak sebagai komponen utama dalam model harga  

### 2. Terapkan dynamic pricing
- Gunakan waktu & kondisi lalu lintas untuk menyesuaikan harga  
- Maksimalkan revenue saat peak hours  

### 3. Fokus pada segmen high-value
- Prioritaskan perjalanan jarak jauh (high revenue contributor)  
- Tingkatkan strategi untuk segmen short trip (promo / pricing)  

### 4. Optimalkan operasional di weekday
- Alokasikan resource lebih banyak pada hari kerja  
- Manfaatkan pola demand untuk efisiensi operasional  

---

## 🛠 Tools yang Digunakan
- Python (Pandas, Matplotlib, Seaborn)  
- Power BI  
- Microsoft Excel  

---

## 📊 Dashboard
Dashboard digunakan untuk:
- Monitoring KPI utama  
- Analisis harga berdasarkan faktor operasional  
- Segmentasi perjalanan  
- Analisis kontribusi revenue  

---

## 📌 Kesimpulan
Analisis menunjukkan bahwa jarak perjalanan merupakan faktor utama dalam menentukan harga, sementara faktor eksternal seperti waktu dan kondisi lalu lintas juga memberikan pengaruh signifikan. Selain itu, segmen perjalanan jarak jauh menjadi kontributor utama revenue.

Insight ini dapat digunakan untuk mengembangkan strategi pricing yang lebih optimal dan meningkatkan profitabilitas bisnis ride-hailing.
