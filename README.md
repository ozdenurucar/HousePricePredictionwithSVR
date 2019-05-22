# HousePricePredictionwithSVR

Bu çalışmada [Kaggle](https://www.kaggle.com/c/house-prices-advanced-regression-techniques) üzerinde yayınlanan gelişmiş regresyon teknikleri ile ev fiyatlarının tahminlemesi yarışması için Support Vector Regresion tekniği kullanılarak bir model oluşturulmuştur.

Veriseti olarak verilen train.csv ve test.csv dosyaları kullanılmıştır.

Tahminleme modeli oluşturulmadan önce veri üzerinde gerekli ön işleme adımları yapılmıştır.

----
    1. Eksik verilerin tamamlanması
    2. Ayrık verilerin tespit edilmesi
    3. Kategorik verilerin Kodlanması
    4. Verilerin ölçeklenmesi
----

Ön işleme işlemleri tamamlandıktan sonra, verilerin birbiri ile olan ilişkisini anlamak amacı ile korelasyon matrisi ile maksimum alakalı özellikler çıkartılmıştır. Burada corr değeri 0.5 eşik değer olarak kabul edilmiştir. 

SalePrice alanı ile 0.5 üzerinde corr değerine sahip olan özellikler belirlenmiştir. 

Daha sonra veriler üzerinde Temel Bileşen Analizi(PCA) uygulanmıştır.

Gerekli ön işleme ve özellik çıkarım işlemleri tammalandıktan sonra Support Vector Machine sınıflandırıcıların Regresyon çeşiti olan Support Vector Regression modeli ile eğitim gerçekleştirilmiştir.

