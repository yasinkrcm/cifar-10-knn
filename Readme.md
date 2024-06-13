# CIFAR-10 ile KNN Projesi

<p align="center">
  <img src="https://miro.medium.com/v2/resize:fit:1100/1*SZnidBt7CQ4Xqcag6rd8Ew.png" alt="CIFAR-10" width="400">
</p>

<p align="center">
  Bu proje, CIFAR-10 veri seti kullanılarak K-Nearest Neighbors (KNN) algoritması ile görüntü sınıflandırma işlemi yapmayı amaçlamaktadır. Proje kapsamında veri ön işleme, model oluşturma, hiperparametre optimizasyonu ve sonuçların değerlendirilmesi adımları gerçekleştirilmiştir.
</p>

## Proje İçeriği

<ol>
  <li><strong>Veri Seti Seçimi</strong>: CIFAR-10 veri seti kullanılmıştır.</li>
  <li><strong>Veri Ön İşleme</strong>:
    <ul>
      <li>Veriler <code>X_train</code>, <code>y_train</code>, <code>X_test</code> ve <code>y_test</code> olarak bölünmüştür.</li>
      <li>Verilerin boyutları yazdırılmıştır.</li>
      <li>Görüntüler görselleştirilmiştir.</li>
      <li>Veriler normalize edilmiştir.</li>
    </ul>
  </li>
  <li><strong>Model Oluşturma ve Eğitme</strong>:
    <ul>
      <li>PCA kullanarak boyut azaltma yapılmıştır.</li>
      <li>GridSearchCV kullanılarak KNN modelinin hiperparametre optimizasyonu yapılmıştır.</li>
      <li>Model eğitilmiş ve test verileri üzerinde tahminler yapılmıştır.</li>
    </ul>
  </li>
  <li><strong>Sonuçların Değerlendirilmesi</strong>:
    <ul>
      <li>Doğruluk, sınıflandırma raporu ve karışıklık matrisi kullanılarak model değerlendirilmiştir.</li>
      <li>Tahmin sonuçları görselleştirilmiştir.</li>
    </ul>
  </li>
</ol>

## Kullanılan Kütüphaneler

<ul>
  <li>numpy</li>
  <li>matplotlib</li>
  <li>tensorflow.keras</li>
  <li>sklearn (scikit-learn)</li>
</ul>

## Veri Seti

<p>
  CIFAR-10 veri seti, 10 farklı sınıfa ait 60,000 renkli görüntüden oluşur. Her sınıfta 6,000 görüntü bulunur. Veri seti, eğitim ve test olmak üzere ikiye ayrılmıştır: 50,000 eğitim ve 10,000 test görüntüsü.
</p>

## KNN Modeli ve Hiperparametre Optimizasyonu

<p>
  Proje kapsamında, KNN algoritması kullanılmış ve GridSearchCV ile en uygun <code>k</code> değeri optimize edilmiştir. Ayrıca, PCA kullanılarak boyut azaltma işlemi yapılmıştır.
</p>

## Sonuçlar

<p>
  Modelin doğruluğu ve diğer değerlendirme metrikleri aşağıda verilmiştir:
</p>

<ul>
  <li><strong>Accuracy</strong>: %30 - %40 arasında</li>
  <li><strong>Classification Report</strong>: Precision, Recall ve F1-Score değerleri</li>
  <li><strong>Confusion Matrix</strong>: Modelin hangi sınıfları doğru veya yanlış sınıflandırdığı gösterilmiştir.</li>
</ul>

## Dosyalar

<ul>
  <li><code>cifar10_knn_pca.ipynb</code>: Proje kodlarının bulunduğu Jupyter Notebook dosyası.</li>
  <li><code>README.md</code>: Proje ile ilgili bilgilerin yer aldığı dosya.</li>
</ul>

## Kurulum ve Çalıştırma

<p>
  Proje dosyasını çalıştırmak için aşağıdaki adımları izleyebilirsiniz:
</p>

<ol>
  <li>Gerekli kütüphaneleri yükleyin:
    <pre><code>pip install numpy matplotlib tensorflow scikit-learn</code></pre>
  </li>
  <li>Jupyter Notebook veya Google Colab kullanarak <code>cifar10_knn_pca.ipynb</code> dosyasını açın ve hücreleri sırasıyla çalıştırın.</li>
</ol>

## Katkıda Bulunanlar

<ul>
  <li>Yasin KARAÇAM - Projeyi geliştiren kişi.</li>
</ul>

## Lisans

<p>
  Bu proje <a href="LICENSE">MIT Lisansı</a> altında lisanslanmıştır.
</p>
