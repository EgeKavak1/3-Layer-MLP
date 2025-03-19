# 3-Layer-MLP

# Banknote Authentication with Neural Network

## Giriş (Introduction)

Bu proje, banknotların sahte olup olmadığını belirlemek için bir yapay sinir ağı modeli geliştirmeyi amaçlamaktadır. Banknotların özellikleri kullanılarak, model sahte ve gerçek banknotları sınıflandırır. Veri seti, banknotların varyans, çarpıklık, basıklık ve entropi gibi özelliklerini içermektedir.

## Yöntem (Methods)

### Veri Seti

Veri seti, `BankNote_Authentication.csv` dosyasından yüklenmiştir. Dosya, banknotların çeşitli özelliklerini ve sınıf etiketlerini içermektedir.

### Model

Model, iki gizli katmanlı bir yapay sinir ağıdır. Her bir gizli katman, ReLU aktivasyon fonksiyonu kullanırken, çıkış katmanı sigmoid aktivasyon fonksiyonu kullanmaktadır. Modelin eğitimi sırasında ileri yayılım, maliyet hesaplama, geri yayılım ve parametre güncelleme adımları gerçekleştirilmiştir.

### Eğitim

Model, `train_test_split` fonksiyonu kullanılarak eğitim ve test verilerine ayrılmıştır. Eğitim sırasında, modelin performansı her 100 iterasyonda bir maliyet fonksiyonu ile değerlendirilmiştir.

## Sonuçlar (Results)

Modelin performansı, doğruluk, kesinlik, geri çağırma ve F1 skoru gibi metriklerle değerlendirilmiştir. Ayrıca, modelin tahmin sonuçları bir karışıklık matrisi ve sınıflandırma raporu ile sunulmuştur.

## Tartışma (Discussion)

Modelin performansı, farklı hiperparametre kombinasyonları ile test edilmiştir. En iyi sonuç, gizli katman boyutları ve eğitim adımları optimize edilerek elde edilmiştir. Modelin doğruluğu, banknotların sahte olup olmadığını belirlemede etkili olduğunu göstermektedir. Yaşanan problemlerden ötürü modelin doğruluğunu artırmayı başaramadım.

## Kullanım (Usage)

1. Gerekli kütüphaneleri yükleyin: `pandas`, `numpy`, `sklearn`.
2. `BankNote_Authentication.csv` dosyasını proje dizinine ekleyin.
3. Python dosyasını çalıştırarak modeli eğitin ve sonuçları değerlendirin.
