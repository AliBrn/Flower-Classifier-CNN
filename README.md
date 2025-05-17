# 🌸 CNN ile Çiçek Sınıflandırma

Beş farklı çiçek türünün sınıfını tahmin eden Evrişimsel Sinir Ağı (CNN) tabanlı bir çiçek görüntü sınıflandırıcısı. Kullanıcılar görüntüleri yükleyebilir ve Streamlit web arayüzü aracılığıyla gerçek zamanlı tahminler alabilir.

-> Bu proje, 5 farklı çiçek türünü sınıflandırmak için Convolutional Neural Network (CNN) kullanır:

- **Daisy**
- **Dandelion**
- **Rose**
- **Sunflower**
- **Tulip**

-> Toplam 4317 görüntü ile eğitilmiştir. Görüntüler 180x180 boyutuna getirilmiş ve normalize edilmiştir.

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

## 🧠 Model Mimarisi

Model şu katmanlardan oluşur:

- 4x Convolution + ReLU
- MaxPooling
- Dropout (Overfitting önleme)
- Flatten
- Dense (Tam bağlı) katmanlar
- Softmax çıkış

---

## 📚 Gereken Kütüphaneler

Projeyi çalıştırmak için gerekli tüm kütüphaneler `requirements.txt` dosyasında listelenmiştir.

Kurmak için:

```bash
pip install -r requirements.txt


## 🧾 Confusion Matrix

Gerçek ve tahmin edilen etiketlerin karşılaştırması:
![Confusion Matrix](flowers/confusion_matrix.png)


🧮 Classification Report
 Class	         Precision	 Recall      F1-Score	    Support
🌼 Daisy	        0.73	      0.82	      0.77	       143
🌾 Dandelion	    0.83	      0.81	      0.82	       200
🌹 Rose         	0.59	      0.67	      0.63	       159
🌻 Sunflower	    0.83	      0.79	      0.81	       148
🌷 Tulip	        0.73	      0.63	      0.68	       213


📊 Genel Performans

Metric	Değer
✅ Accuracy	0.74
🧾 Macro Avg	0.74
🧮 Weighted Avg	0.74

🔍 Model özellikle dandelion ve sunflower sınıflarında yüksek başarı göstermiştir.
🌹 "Rose" sınıfında başarı oranı görece daha düşüktür, bu sınıfta veri artırımı yapılabilir.

📂 Klasör Yapısı

Images/ — Veri setinde kullanılan çiçek fotoğrafları

Sample/ — Modeli test etmek için seçilmiş örnek fotoğraflar


## 🚀 Projeyi Çalıştırmak

- `model_cicek_tahmini.ipynb` dosyasını açarak modeli inceleyebilir ve çalıştırabilirsiniz.
- Canlı tahminler için Streamlit arayüzü (`app.py`) kullanılabilir.

```bash
streamlit run app.py


