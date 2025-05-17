# 🌸 CNN ile Çiçek Sınıflandırma

Beş farklı çiçek türünün sınıfını tahmin eden Evrişimsel Sinir Ağı (CNN) tabanlı bir çiçek görüntü sınıflandırıcısı. Kullanıcılar görüntüleri yükleyebilir ve Streamlit web arayüzü aracılığıyla gerçek zamanlı tahminler alabilir.

Bu proje, 5 farklı çiçek türünü sınıflandırmak için Convolutional Neural Network (CNN) kullanır:

- **Daisy**
- **Dandelion**
- **Rose**
- **Sunflower**
- **Tulip**

Toplam 4317 görüntü ile eğitilmiştir. Görüntüler 180x180 boyutuna getirilmiş ve normalize edilmiştir.

---
## 📁 Veri Kümesi

- Görüntü sayısı: 4317
- Görüntü boyutu: 180x180
- Veri tek klasörde ve alt klasörlerde sınıflara ayrılmıştır:
flowers/
├── daisy/
├── dandelion/
├── rose/
├── sunflower/
└── tulip/

### 🧾 Confusion Matrix

Gerçek ve tahmin edilen etiketlerin karşılaştırması:
![Confusion Matrix](confusion_matrix.png)


