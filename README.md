# Hayvan Sınıflandırma Projesi

Bu proje, belirli hayvan sınıflarını sınıflandırmak için bir Convolutional Neural Network (CNN) modeli kullanır. Veri seti manipüle edilmiş ve renk sabitliği uygulanmış test setleri üzerinde modelin performansını değerlendirir.

## Proje Özeti
•⁠  ⁠*Veri Seti*: [Animals with Attributes 2](https://www.kaggle.com/datasets/rrebirrth/animals-with-attributes-2)
•⁠  ⁠*Amaç*: Modelin manipülasyonlara dayanıklılığını ve renk sabitliği algoritmalarının etkisini değerlendirmek.
•⁠  ⁠*Model Türü*: Convolutional Neural Network (CNN).
•⁠  ⁠*Kütüphaneler*: TensorFlow, Keras, NumPy, Matplotlib, PIL, OpenCV.

## Kullanılan Teknikler
1.⁠ ⁠*Veri Ön İşleme*:
   - Görüntülerin yeniden boyutlandırılması (128x128 piksel).
   - Piksel değerlerinin normalize edilmesi.
   - Eğitim (%70) ve test (%30) veri setlerinin ayrılması.
   
2.⁠ ⁠*Veri Artırma (Augmentation)*:
   - Döndürme, kaydırma, yakınlaştırma ve yatay çevirme gibi manipülasyonlar.

3.⁠ ⁠*Model Eğitimi*:
   - CNN modeli kullanılarak eğitim.
   - Modelin ⁠ categorical_crossentropy ⁠ kayıp fonksiyonu ile optimize edilmesi.

4.⁠ ⁠*Manipüle Edilmiş Test Seti*:
   - Test setine parlaklık manipülasyonu uygulanmıştır.

5.⁠ ⁠*Renk Sabitliği*:
   - Gray World algoritması ile manipülasyon etkilerinin azaltılması hedeflenmiştir.

## Test Seti Performansı
| Test Seti            | Doğruluk Oranı (%) |
|-----------------------|--------------------|
| Normal               | *56.62*          |
| Manipüle Edilmiş     | *47.69*          |
| Renk Sabitliği       | *40.67*          |

## Kurulum
1.⁠ ⁠*Gerekli Kütüphaneler*:
   - Projede kullanılan kütüphaneler:
     ⁠ bash
     pip install tensorflow numpy matplotlib pillow opencv-python
      ⁠

2.⁠ ⁠*Google Colab Kullanımı*:
   - [Google Colab](https://colab.research.google.com/) üzerinde bu projeyi çalıştırabilirsiniz.
   - ⁠ .ipynb ⁠ dosyasını Colab'da açarak çalıştırın.

3.⁠ ⁠*Manuel Çalıştırma*:
   - Projeyi bilgisayarınıza klonlayın:
     ⁠ bash
     git clone https://github.com/kullaniciadi/projeadi.git
      ⁠
   - Proje dizinine gidin ve gerekli kütüphaneleri yükleyin.

## Lisans
Bu proje MIT Lisansı altında paylaşılmıştır. Daha fazla bilgi için [LICENSE](LICENSE) dosyasına bakabilirsiniz.
