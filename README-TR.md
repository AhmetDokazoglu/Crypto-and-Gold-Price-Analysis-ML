# Kripto ve Altın Fiyatlarının Analizi ve Makine Öğrenmesi ile Öngörüsü (2015–2025)

# 🎯 Proje Özeti

# 

# Bu proje, Bitcoin, Ethereum, Binance Coin, Ripple, Cardano, Dogecoin, Solana ve Altın (Gold/USD) fiyatlarını 2015–2025 dönemi boyunca analiz ederek, makine öğrenmesi algoritmaları ile kısa vadeli fiyat yönü (artış / düşüş) tahminleri yapmayı amaçlamaktadır.

# Amaç, kripto paraların “dijital altın” olup olamayacağını anlamak ve klasik makine öğrenmesi modellerinin finansal zaman serilerine uygulanabilirliğini göstermektir.

# 

# 📊 Kullanılan Veri Seti

# 

# Kaynak: Kaggle - Crypto and Gold Prices Dataset (2015–2025)

# 

# Özellik	Açıklama

# Dönem	2015 Ocak – 2025 Ocak

# Varlıklar	Bitcoin, Ethereum, BNB, XRP, ADA, DOGE, SOL, Gold

# Frekans	Günlük kapanış fiyatı

# Hedef	Ertesi gün fiyat artışı (1) / düşüşü (0)

# 🧠 Kullanılan Modeller

# 

# Lojistik Regresyon (Logistic Regression)

# 

# K-En Yakın Komşu (KNN)

# 

# Destek Vektör Makinesi (SVM, RBF Kernel)

# 

# Random Forest

# 

# Her model aynı veri setinde, aynı özelliklerle (ret\_1d, ret\_7d, vol\_7d, ma30\_dev, mom\_10) test edilmiştir.

# 

# ⚙️ Özellik (Feature) Mühendisliği

# 

# Veri setinden türetilen teknik göstergeler:

# 

# Özellik	Açıklama

# ret\_1d	Günlük getiri

# ret\_7d	7 günlük ortalama getiri

# vol\_7d	7 günlük volatilite (standart sapma)

# ma30\_dev	30 günlük ortalamadan sapma

# mom\_10	10 günlük momentum göstergesi

# 

# Bu göstergeler klasik teknik analizden türetilmiştir ve kısa vadeli tahmin için sinyal üretir.

# 

# 🧩 Kod Akışı

# 

# Verinin okunması ve tarihlerin dönüştürülmesi

# 

# Eksik verilerin temizlenmesi

# 

# Özelliklerin üretilmesi

# 

# Train/Test ayrımı (2015–2021 → Train, 2022–2025 → Test)

# 

# Modellerin eğitilmesi

# 

# Performans karşılaştırması (Accuracy, Confusion Matrix, Heatmap)

# 

# 📈 Sonuçlar ve Bulgular

# Model	Bitcoin	Ethereum	Gold	BNB

# Logistic Regression	0.68	0.68	0.68	0.68

# KNN	0.66	0.66	0.66	0.66

# SVM	0.68	0.68	0.68	0.68

# Random Forest	0.65	0.65	0.65	0.65

# 

# En yüksek doğruluk: Logistic Regression \& SVM (%68)

# 

# En dengeli model: Random Forest

# 

# Düşüş tahminleri zayıf, artış tahminleri daha başarılı

# 

# 📊 Görsel çıktılar:

# 

# Confusion Matrix (her model için)

# 

# Accuracy Heatmap (Models × Assets)

# 

# Feature Importance (Random Forest)

# 

# 💡 Öne Çıkan Katkılar

# 

# Kripto ve altın fiyatlarının karşılaştırmalı analizi

# 

# Klasik ML modelleri ile finansal serilerde öngörü denemesi

# 

# 10 yıllık uzun dönem veriyle trend ve volatilite farklarının ortaya konması

# 

# 🔍 Gelecekteki Geliştirmeler

# 

# Derin öğrenme modelleri (LSTM, GRU, Prophet)

# 

# Makroekonomik göstergelerle ilişkilendirme (enflasyon, faiz, para arzı)

# 

# Çoklu para birimi analizi (USD, EUR, TRY bazlı fiyatlar)

# 

# 📚 Kaynaklar

# 

# Kaggle Dataset

# 

# Nakamoto, S. (2008). Bitcoin: A Peer-to-Peer Electronic Cash System.

# 

# Dyhrberg, A. H. (2016). Bitcoin, gold and the dollar – A GARCH volatility analysis.

# 

# Corbet et al. (2019). Cryptocurrencies as a financial asset: A systematic analysis.

# 

# 👨‍💻 Hazırlayan

# 

# Yunus Ahmet Dokazoğlu

# Data Analyst \& Economist

# 📧 ahmetdokazoglu@example.com

# 

# 📍 Ankara, Türkiye

