# mnist-rakam-tanima
MNIST veri setiyle eğitilen modelin dış görsellerle test edilmesi projesi
# 🎓 Final Proje: Harici Görselle Rakam Tanıma (MNIST)

Bu proje, **MNIST veri seti** kullanılarak eğitilen bir yapay sinir ağının, dışarıdan yüklenen el yazısı rakam görsellerini tanımasını sağlar.

## 🧠 Kullanılan Teknolojiler

- Python
- TensorFlow / Keras
- NumPy, Matplotlib
- PIL (Python Imaging Library)

## 🗂️ Dosya Açıklamaları

- `Final_Proje_Harici_Gorsel_Tanima.ipynb`: Model eğitimi, dış görselle test ve tahmin süreci.
- `mnist_model.h5`: Eğitilmiş model dosyası.
- `rakam-5.jpg`: Test için kullanılan dış görsel.
- `README.md`: Açıklayıcı bu belge.

## 🧪 Proje Adımları

1. MNIST veri setiyle model eğitilir.
2. Model `.h5` dosyasına kaydedilir.
3. Kullanıcı, dışarıdan bir el yazısı rakam (`rakam-5.jpg`) yükler.
4. Görsel 28x28 boyutuna getirilip griye çevrilir.
5. Model bu görseli tanır ve sonucu verir.

## 📷 Görsel İşleme

- Görsel: gri tonlamaya çevrilir (`convert('L')`)
- 28x28 piksel boyutuna ölçeklenir
- Siyah-beyaz kontrastı ters çevrilir (arka plan siyah, rakam beyaz olmalı)

## 🔍 Örnek Tahmin

```bash
Tahmin edilen rakam: 5
