# 🛰️ K.O.R.U. (Korelasyon ve Optimize Edilmiş Rota Uyumu)

Türk uydularını uzay çöplerinden korumak için tasarlanmış, XGBoost destekli yörünge ve çarpışma önleme sistemi.

## 📝 Proje Özeti
Günümüzde artan uzay çöpleri (space debris), aktif uydularımız için büyük bir tehdit oluşturmaktadır. K.O.R.U. projesi, ESA, CelesTrak, Space-Track ve NOAA verilerini anlık olarak işleyerek olası çarpışma risklerini önceden tespit eden otonom bir karar destek sistemidir.

## ✨ Temel Özellikler ve Senaryolar
Makine öğrenmesi modelimiz, risk durumunu 3 ana senaryoda değerlendirir:
* **🔴 SENARYO 1 (Kritik Durum - Çöp Yakında ve Alçakta):** Sistem anlık hız ve süre hesaplamasıyla **Acil Manevra** komutu verir.
* **🟡 SENARYO 2 (Orta Risk - Çöp Alt Tarafında):** Sistem rotayı güvenceye almak için **Manevra Hazırlıklarını** başlatır.
* **🟢 SENARYO 3 (Düşük Risk - Çöp Uzakta):** Otonom **Takip** devam eder.

## 🛠️ Kullanılan Teknolojiler
* **Makine Öğrenmesi:** Python, XGBoost (Yüksek Doğruluk, Minimum Overfitting)
* **Veri Kaynakları:** ESA, CelesTrak, Space-Track.org, NOAA
* **Arayüz:** Kullanıcı dostu dinamik web paneli (Uydu/çöp filtreleme, yörünge seçimi)
