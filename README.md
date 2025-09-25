# 🍃 Leaf Disease Classification

## 🎯 Projenin Amacı

Bu proje, derin öğrenme yöntemleriyle bitki yapraklarındaki hastalıkları veya sağlıklı oluşunu sınıflandırmayı amaçlamaktadır. Aynı zamanda çeşitli tablolar, karşılaştırmalar ve matrisler yoluyla en optimum sonucu görebilmeyi hedeflemektedir.

## 📊 Veri Seti Hakkında

- **Kaynak:** Kaggle üzerinden [Leaf Disease Dataset](https://www.kaggle.com/datasets/smaranjitghose/corn-or-maize-leaf-disease-dataset) kullanılmıştır.
- **Sınıflar:** Toplamda 4 farklı sınıf bulunmaktadır. Veri seti Blight sınıfı 1146 Common_Rust 1306 Gray_Leaf_Spot 574 Healthy 1162 adet olmak üzere toplamda 4188 adet görselden oluşmaktadır.
- **Önişleme:** Resimler yeniden boyutlandırılmış ve normalize edilmiştir.
- **Veri Çoğaltma:** Resim döndürme, yatay ve dikey çevirme gibi tekniklerle veri artırımı yapılmıştır.
- **Veri Paylaştırma:** Veriler train, validation ve test olmak üzere 3 ayrı parçaya bölünmüştür.

## ⚙️ Kullanılan Yöntemler

- **Model:** Evrişimsel Sinir Ağları (CNN) mimarisi kullanılmıştır.    
- **Eğitim:** Model, 20 epoch boyunca eğitilmiştir.  
- **Değerlendirme:** Modelin başarımı accuracy, precision, recall ve f1-score metrikleri ile değerlendirilmiştir.
- **Augmentation Tekniği:** Görseller üstünde değişiklik yapabilmek için "ImageDataGenerator" kullanılmıştır.
- **Veriyi Bölme Tekniği:** Veriyi train, validation ve test olarak bölebilmek için "train_test_split" kullanılmıştır.
- **Model Oluşturma Tekniği:** Model oluşturulurken "Sequential API" tekniği kullanılmıştır.
- **Overfitting Önlem Alma:** Overfitting'i engellemek için Dropout, EarlyStopping, Data Augmentation ve L2 Regularization teknikleri kullanılmıştır.
- **Eğitimi Stabilize Etme:** Model eğitimini daha kararlı ve verimli hale getirmek için ReduceLROnPlateau ve BatchNormalization teknikleri kullanılmıştır.

## 📈 Deneysel Sonuçlar

- **En İyi Test Doğruluğu:** 0.9212
- **En İyi Test Kaybı:** 0.2420
- **Karmaşıklık Matrisi:** Modelin sınıflandırma başarısını gösteren karmaşık matris görselleştirilmiştir.
- **Accuracy-Loss Grafiği:** Model eğitilirken çıkan sonuçlara göre acc-val_acc ve loss-val_loss değerlerinin değişimi gösterilir.
- **Augmentation Deney:** Train datasına augmentation uyguladıktan sonra örnek yazdırma.
- **Heatmap Görselleştirme:** Modelin karar alırken görseller üzerinde hangi bölgelere baktığı Grad-CAM kullanılarak heatmap görselleştirmesi yapılmıştır.
- **Hiperparametre Optimizasyonu:** Model eğitilirken 2 farklı dropout oranı denenerek farklı sonuçlar elde edilmiştir.

## 🚀 Nasıl Çalıştırılır

1. **Ortam Kurulumu:**
   ```bash
   pip install -r requirements.txt

2. **Notebook Çalıştırma:**
   - `leaf-disease-classification.ipynb` dosyasını açın.

3. **Model Eğitimi**
   - Notebook içerisindeki hücreleri sırasıyla çalıştırarak model eğitimini başlatın.

4. **Model Değerlendirme**
   - Eğitim tamamlandıktan sonra modelin başarımını değerlendirin.

## 🔗 Kaggle Notebook
Proje linki: [Leaf Disease Classification](https://www.kaggle.com/code/skutukte/leaf-disease-classification)




