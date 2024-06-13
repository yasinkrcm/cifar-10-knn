
<p align="center">
  <img src="https://miro.medium.com/v2/resize:fit:1100/1*SZnidBt7CQ4Xqcag6rd8Ew.png" alt="CIFAR-10" width="600">
</p>

<h1 align="center">CIFAR-10 ile KNN Projesi</h1>

<p align="center">
  <b>Görüntü sınıflandırma işlemi için K-Nearest Neighbors (KNN) algoritması kullanımı.</b>
</p>

<p align="center">
  <a href="#proje-içeriği">Proje İçeriği</a> •
  <a href="#kullanılan-kütüphaneler">Kullanılan Kütüphaneler</a> •
  <a href="#veri-seti">Veri Seti</a> •
  <a href="#knn-modeli-ve-hiperparametre-optimizasyonu">KNN Modeli ve Hiperparametre Optimizasyonu</a> •
  <a href="#sonuçlar">Sonuçlar</a> •
  <a href="#kurulum-ve-çalıştırma">Kurulum ve Çalıştırma</a> •
  <a href="#katkıda-bulunanlar">Katkıda Bulunanlar</a> •
  <a href="#lisans">Lisans</a>
</p>

<p align="center">
  <a href="https://github.com/YasinKrcm/cifar-10-knn/releases">
    <img src="https://img.shields.io/github/v/release/YasinKrcm/cifar-10-knn.svg?style=flat-square" alt="Releases">
  </a>
  <a href="https://github.com/YasinKrcm/cifar-10-knn/blob/main/LICENSE">
    <img src="https://img.shields.io/github/license/YasinKrcm/cifar-10-knn.svg?style=flat-square" alt="License">
  </a>
  <a href="https://github.com/YasinKrcm/cifar-10-knn/issues">
    <img src="https://img.shields.io/github/issues/YasinKrcm/cifar-10-knn.svg?style=flat-square" alt="Issues">
  </a>
  <a href="https://github.com/YasinKrcm/cifar-10-knn/pulls">
    <img src="https://img.shields.io/github/issues-pr/YasinKrcm/cifar-10-knn.svg?style=flat-square" alt="Pull Requests">
  </a>
</p>

---

## Proje İçeriği

- **Veri Seti Seçimi**: CIFAR-10 veri seti kullanılmıştır.
- **Veri Ön İşleme**:
  - Veriler `X_train`, `y_train`, `X_test` ve `y_test` olarak bölünmüştür.
  - Verilerin boyutları yazdırılmıştır.
  - Görüntüler görselleştirilmiştir.
  - Veriler normalize edilmiştir.
- **Model Oluşturma ve Eğitme**:
  - PCA kullanarak boyut azaltma yapılmıştır.
  - GridSearchCV kullanılarak KNN modelinin hiperparametre optimizasyonu yapılmıştır.
  - Model eğitilmiş ve test verileri üzerinde tahminler yapılmıştır.
- **Sonuçların Değerlendirilmesi**:
  - Doğruluk, sınıflandırma raporu ve karışıklık matrisi kullanılarak model değerlendirilmiştir.
  - Tahmin sonuçları görselleştirilmiştir.

## Kullanılan Kütüphaneler

- numpy
- matplotlib
- tensorflow.keras
- sklearn (scikit-learn)

## Veri Seti

CIFAR-10 veri seti, 10 farklı sınıfa ait 60,000 renkli görüntüden oluşur. Her sınıfta 6,000 görüntü bulunur. Veri seti, eğitim ve test olmak üzere ikiye ayrılmıştır: 50,000 eğitim ve 10,000 test görüntüsü.

## KNN Modeli ve Hiperparametre Optimizasyonu

Proje kapsamında, KNN algoritması kullanılmış ve GridSearchCV ile en uygun `k` değeri optimize edilmiştir. Ayrıca, PCA kullanılarak boyut azaltma işlemi yapılmıştır.

## Sonuçlar

Modelin doğruluğu ve diğer değerlendirme metrikleri aşağıda verilmiştir:

- **Accuracy**: %30 - %40 arasında
- **Classification Report**: Precision, Recall ve F1-Score değerleri
- **Confusion Matrix**: Modelin hangi sınıfları doğru veya yanlış sınıflandırdığı gösterilmiştir.

## Kurulum ve Çalıştırma

1. Gerekli kütüphaneleri yükleyin:
   ```bash
   pip install numpy matplotlib tensorflow scikit-learn
   ```

2. Jupyter Notebook veya Google Colab kullanarak `cifar10_knn_pca.ipynb` dosyasını açın ve hücreleri sırasıyla çalıştırın.

## Katkıda Bulunanlar

- **Yasin KARAÇAM** - Projeyi geliştiren kişi.
  - [GitHub](https://github.com/yasinkrcm)
  - [LinkedIn](https://www.linkedin.com/in/yasin-karacamm/)

## Lisans

Bu proje [MIT Lisansı](LICENSE) altında lisanslanmıştır.
