
# Shill Bidding Tespiti: Veri Madenciliği Yaklaşımıyla Sınıflandırma Analizi

Bu proje, **Bursa Teknik Üniversitesi - Bilgisayar Mühendisliği** bölümünde verilen **BLM463 Veri Madenciliğine Giriş** dersi kapsamında hazırlanmıştır.

## 📌 Proje Özeti

Çevrim içi açık artırma sistemlerinde kullanıcıları manipüle eden "shill bidding" (sahte teklif verme) davranışını tespit etmek için çeşitli makine öğrenmesi algoritmaları kullanılarak sınıflandırma modeli geliştirilmiştir.

## 🎯 Proje Hedefleri

- Sahte teklif veren kullanıcıları tespit etmek
- Farklı sınıflandırma algoritmalarını karşılaştırmak
- Hiperparametre optimizasyonu uygulamak
- Veri madenciliği sürecinin her aşamasını detaylandırmak

## 📁 Kullanılan Veri Seti

- **Kaynak:** [shill_bidding_dataset.csv](https://archive.ics.uci.edu/dataset/562/shill+bidding+dataset)
- **Gözlem sayısı:** 6321
- **Özellik sayısı:** 38
- **Hedef değişken:** `Class` (0 = normal, 1 = shill bidder)

## 🧰 Kullanılan Kütüphaneler

- `pandas`, `numpy` – veri işleme
- `matplotlib`, `seaborn` – görselleştirme
- `scikit-learn` – modelleme ve metrikler
- `imbalanced-learn` – SMOTE uygulaması

## 🔍 Veri Ön İşleme Adımları

- Eksik değer analizi
- Aykırı değerlerin Winsorize ile sınırlandırılması
- Label Encoding (kategorik değişkenler için)
- StandardScaler ile normalizasyon
- Korelasyon analizi ve yüksek korelasyonlu değişkenlerin çıkarılması

## 📊 Sınıflandırma Algoritmaları

1. **Random Forest**
2. **Support Vector Machine (SVM)**
3. **K-Nearest Neighbors (KNN)**

Her model için **GridSearchCV** ile hiperparametre optimizasyonu yapılmıştır.

## ⚙️ Performans Sonuçları

| Model                | Accuracy | Precision | Recall | F1 Score |
|----------------------|----------|-----------|--------|----------|
| Random Forest        | 0.9968   | 0.9965    | 0.9968 | 0.9968   |
| Random Forest (Opt)  | 0.9976   | 0.9976    | 0.9976 | 0.9976   |
| SVM                  | 0.9818   | 0.9845    | 0.9818 | 0.9824   |
| SVM (Opt)            | 0.9921   | 0.9924    | 0.9921 | 0.9922   |
| KNN                  | 0.9834   | 0.9851    | 0.9834 | 0.9838   |
| KNN (Opt)            | 0.9826   | 0.9842    | 0.9826 | 0.9830   |

✅ En iyi sonuç **Optimize Edilmiş Random Forest** modeli ile elde edilmiştir.

## 📈 Gelecek Çalışmalar

- Derin öğrenme yaklaşımlarının entegrasyonu
- Daha geniş ve güncel veri setlerinin kullanılması
- Hibrit ve istatistiksel temelli sistemlerin denenmesi

## 🗃️ Proje Yapısı

```
📂 shill-bidding-detection
├── codes/
│   └── main.ipynb
├── dataset/
│   └── shill_bidding_dataset.csv
├── projectvenv
├── report/
│   └── BLM463_Proje_İbrahimSemihTemiz_21360859054.pdf
├── README.md
└── 
```


## 🎥 Proje Tanıtım Videosu

📽️ [Veri Madenciliği ile Shill Bidding Tespiti]([https://www.youtube.com/watch?v=video-linki](https://youtu.be/yy22st9vx0Q))

## 👤 Hazırlayan

- İbrahim Semih Temiz  
- Bursa Teknik Üniversitesi – Bilgisayar Mühendisliği
