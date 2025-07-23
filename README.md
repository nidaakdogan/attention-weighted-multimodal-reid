# 🎓 Attention-Based Weighted Multi-Modal Person Re-Identification

Bu proje, yüksek lisans tez çalışmam kapsamında geliştirilmiş olan **Dikkat Tabanlı Ağırlıklandırılmış Çoklu-Modaliteli Kişi Yeniden Tanıma (Re-ID)** sistemidir. RGB ve Sketch modalitelerini birleştirerek, kişilerin farklı kıyafetlerle ve farklı açılardan yüksek doğrulukla yeniden tanınmasını amaçlamaktadır.

---

## 📌 Projenin Amacı

Klasik kişi yeniden tanıma sistemleri, tek bir görüntü modalitesine bağlı kalmakta ve çevresel değişimlerde başarısız olabilmektedir. Bu projede amaç; **RGB + Sketch** görüntülerini kullanarak **attention mekanizmasıyla ağırlıklandırılmış bir multi-modal yapıyı** oluşturmak ve kişi tanıma başarımını artırmaktır.

---

## 🧠 Kullanılan Mimariler

| Model                           | Açıklama |
|--------------------------------|----------|
| `rgbmodal_vgg16_pynb.ipynb`    | VGG16 tabanlı sadece RGB girişli model |
| `RgbModal_Resnet50.ipynb`      | ResNet50 tabanlı sadece RGB girişli model |
| `vgg16multimodal.ipynb`        | VGG16 tabanlı RGB + Sketch multi-modal model |
| `Resnet_multimodal_son.ipynb`  | ResNet50 tabanlı RGB + Sketch multi-modal model |
| `weighted_attention.ipynb`     | Ağırlıklı dikkat mekanizması ile geliştirilen Multi-Modal sistem |

---

## 🗂️ Veri Seti: PRCC (Person Re-ID under Clothing Change Challenge)

- **probA:** RGB görüntüleriyle test yapılır.
- **probB:** Aynı kişi ve aynı kıyafet kombinasyonu.
- **probC:** Aynı kişi, farklı kıyafet kombinasyonları.

Veri seti, kıyafet değişimine karşı dayanıklı yeniden tanıma sistemleri için kullanılır.

---

---

## 🛠️ Kullanılan Teknolojiler

| Katman     | Teknoloji                      |
|------------|--------------------------------|
| Backend    | Python (Jupyter Notebook)      |
| DL Lib.    | TensorFlow, Keras, NumPy       |
| Görselleştirme | Matplotlib, Seaborn       |
| Versiyon   | Git & GitHub                   |

---

## 📁 Proje Yapısı


- `vgg16multimodal.ipynb`  
  VGG16 mimarisi kullanılarak RGB ve Sketch görüntülerinin birlikte işlendiği temel multi-modal kişi yeniden tanıma modeli.

- `rgbmodal_vgg16_pynb.ipynb`  
  Sadece RGB görüntüleriyle çalışan VGG16 tabanlı tek modaliteli model.

- `RgbModal_Resnet50.ipynb`  
  Sadece RGB görüntüleri kullanan ResNet50 mimarisine sahip model.

- `Resnet_multimodal_son.ipynb`  
  ResNet50 mimarisi ile hem RGB hem de Sketch modalitelerini kullanan gelişmiş multi-modal yapı.


- `Attention-Based Weighted Multi-Modal Person.pdf`  
RGB ve Sketch verilerinin dikkat mekanizmalarıyla ağırlıklandırılarak birleştirildiği, performansı yüksek final model.

- `data/PRCC/`  
  PRCC veri kümesinin kullanıldığı test senaryolarını (probe A, probe B, probe C) içeren dizin yapısı:
  
  - `probe A/`: RGB görüntülerle test  
  - `probe B/`: Aynı kişi, aynı kıyafet kombinasyonu  
  - `probe C/`: Aynı kişi, farklı kıyafet kombinasyonu


