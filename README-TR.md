# 🪙 Kripto ve Altın Fiyatlarının Analizi ve Makine Öğrenmesi ile Öngörüsü (2015–2025)

### 🎯 Proje Özeti
Bu proje, **Bitcoin, Ethereum, Binance Coin, Ripple, Cardano, Dogecoin, Solana** ve **Altın (USD/ons)** fiyatlarını **2015–2025** yılları arasında analiz ederek, **makine öğrenmesi algoritmaları** ile kısa vadeli fiyat yönünü (artış / düşüş) tahmin etmeyi amaçlamaktadır.  
Amaç, kripto paraların “dijital altın” olarak değerlendirilebilip değerlendirilemeyeceğini araştırmak ve klasik makine öğrenmesi modellerinin finansal zaman serilerindeki başarımını ölçmektir.

---

## 📊 Veri Seti Bilgileri
**Kaynak:** [Kaggle – Crypto and Gold Prices Dataset (2015–2025)](https://www.kaggle.com/datasets/muhamedumarjamil/crypto-and-gold-prices-dataset-20152025)

| Özellik | Açıklama |
|----------|-----------|
| **Dönem** | 2015 Ocak – 2025 Ocak |
| **Varlıklar** | Bitcoin, Ethereum, BNB, XRP, ADA, DOGE, SOL, Gold |
| **Frekans** | Günlük kapanış fiyatı |
| **Hedef Değişken** | Ertesi gün fiyat yönü → 1 (Artış), 0 (Düşüş) |

---

## 🧠 Kullanılan Modeller
1. **Lojistik Regresyon (Logistic Regression)**  
2. **K-En Yakın Komşu (KNN)**  
3. **Destek Vektör Makinesi (SVM, RBF Kernel)**  
4. **Random Forest**

Tüm modeller aynı dönem ve aynı özelliklerle eğitilip test edilmiştir, böylece adil bir karşılaştırma yapılmıştır.

---

## ⚙️ Özellik (Feature) Mühendisliği
Veri setinden türetilen teknik göstergeler:

| Özellik | Açıklama |
|----------|-----------|
| `ret_1d` | Günlük getiri |
| `ret_7d` | 7 günlük ortalama getiri |
| `vol_7d` | 7 günlük volatilite (standart sapma) |
| `ma30_dev` | 30 günlük hareketli ortalamadan sapma |
| `mom_10` | 10 günlük momentum göstergesi |

Bu göstergeler hem trendi hem de volatilite davranışını yansıtarak kısa vadeli sinyal sağlar.

---

## 🧩 Kod Akışı
1. Veri setinin okunması ve temizlenmesi  
2. Özelliklerin ve etiketlerin üretilmesi  
3. Train/Test ayrımı (2015–2021 → Eğitim, 2022–2025 → Test)  
4. Modellerin eğitilmesi  
5. Performans ölçümü (Doğruluk oranı, Karışıklık Matrisi)  
6. Görselleştirmeler (Isı Haritası, Özellik Önemleri, Model Kıyasları)

---

## 📈 Sonuçlar
| Model | BTC | ETH | GOLD | BNB |
|--------|-----|-----|------|-----|
| Lojistik Regresyon | 0.68 | 0.68 | 0.68 | 0.68 |
| KNN | 0.66 | 0.66 | 0.66 | 0.66 |
| SVM | 0.68 | 0.68 | 0.68 | 0.68 |
| Random Forest | 0.65 | 0.65 | 0.65 | 0.65 |

- **En yüksek doğruluk:** Logistic Regression & SVM (~%68)  
- **En dengeli model:** Random Forest  
- Tüm modeller artış günlerinde başarılı, düşüş günlerinde zayıf performans göstermiştir.

---

## 💡 Temel Bulgular
- Kripto varlıklar altına kıyasla **daha yüksek volatiliteye** sahip ancak **daha yüksek getiri potansiyeli** taşımaktadır.  
- Basit teknik göstergelerle bile ML modelleri kısa vadeli hareketleri yakalayabilmektedir.  
- Model karşılaştırmaları, yatırımcıların **risk-getiri dengesini** daha iyi anlamasına yardımcı olur.

---

## 🚀 Gelecekteki Geliştirmeler
- **Derin öğrenme modelleri** (LSTM, GRU, Prophet) ile ileri zaman serisi tahminleri  
- **Makroekonomik değişkenlerin** (enflasyon, faiz, para arzı vb.) entegrasyonu  
- Çoklu para birimi analizi (USD, EUR, TRY karşılaştırmaları)

---

## 📚 Kaynaklar
- [Kaggle Veri Seti](https://www.kaggle.com/datasets/muhamedumarjamil/crypto-and-gold-prices-dataset-20152025)  
- Nakamoto, S. (2008). *Bitcoin: A Peer-to-Peer Electronic Cash System.*  
- Dyhrberg, A. H. (2016). *Bitcoin, gold and the dollar – A GARCH volatility analysis.*  
- Corbet et al. (2019). *Cryptocurrencies as a financial asset: A systematic analysis.*

---

## 👨‍💻 Hazırlayan
**Yunus Ahmet Dokazoğlu**  
_Data Analyst & Economist_  
📍 Ankara, Türkiye  
📫 [LinkedIn](https://www.linkedin.com/in/ahmet-dokazo%C4%9Flu-9660b2346/) • [GitHub](https://github.com/AhmetDokazoglu)
