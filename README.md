# Training for Pertamina Intern Preparation: Fraud Detection EDA

**Penulis:** Meidy Afif Maulana  
**Target Posisi:** Data Analyst / Internal Audit Intern di Pertamina  
**Tech Stack:** Python, Pandas, NumPy, Matplotlib, Seaborn  

## Ringkasan Proyek
Repository ini berisi tahapan Exploratory Data Analysis (EDA) dari proyek deteksi fraud keuangan. Proyek ini aku kerjakan khusus sebagai persiapan untuk program magang di Pertamina, dengan fokus mencari anomali dan menganalisis data dari sudut pandang internal audit.

Dataset yang digunakan memiliki lebih dari 6,3 juta baris log transaksi keuangan yang direkam selama 31 hari.

## Temuan Utama
1. **Modus Operandi Terstruktur:** 100% dari 8.213 kasus fraud hanya menggunakan metode TRANSFER dan CASH_OUT untuk memutus jejak pelacakan.
2. **Eksploitasi Celah Sistem:** Melalui perhitungan logika saldo, aku menemukan bahwa pelaku bisa menarik uang dalam jumlah besar tanpa mengurangi saldo awal mereka di sistem.
3. **Kegagalan Sistem Lama:** Sistem alarm bawaan (isFlaggedFraud) terbukti gagal mendeteksi mayoritas serangan ini, membuktikan bahwa sistem berbasis aturan (rule-based) saja sudah tidak memadai.
4. **Jam Rawan Operasi:** Aktivitas fraud memuncak antara jam 02:00 sampai 04:00 pagi. Ini menunjukkan bahwa pelaku menargetkan jam-jam di mana pengawasan sedang lemah atau kemungkinan menggunakan script otomatis (bot).

## Langkah Selanjutnya
* Melakukan Data Preprocessing dan Feature Encoding.
* Menangani Imbalanced Data menggunakan teknik SMOTE.
* Membangun model klasifikasi Machine Learning untuk mendeteksi fraud secara otomatis.
