# 🧠 Brain Tumor Detection Using Deep Learning (CNN)

Bu proje, Beyin MR (Manyetik Rezonans) görüntülerini analiz ederek beyin tümörü tespiti ve sınıflandırması yapan Evrişimli Sinir Ağı (CNN) tabanlı bir derin öğrenme uygulamasıdır.

---

## 📂 Veri Seti (Dataset)
Projede kullanılan veri seti Kaggle üzerinden temin edilmiştir:
* **Veri Seti:** [Brain MRI Images for Brain Tumor Detection (Kaggle)](https://www.kaggle.com/datasets/navoneel/brain-mri-images-for-brain-tumor-detection)
* **İçerik:** Tümörlü (`yes`) ve tümörsüz (`no`) olarak etiketlenmiş beyin MR görüntülerinden oluşmaktadır.
* **Veri Bölünmesi:** `train_test_split` (%80 Eğitim / %20 Test) ve `ImageDataGenerator` ile `224x224x3` (RGB) formatında işlenmiştir.

---

## 📊 Model Performansı ve Sonuçlar

Modelin eğitim ve test aşamalarında elde ettiği doğruluk (accuracy) ve kayıp (loss) değerleri:

| Metrik | Eğitim (Train) | Test |
| :--- | :---: | :---: |
| **Accuracy (Doğruluk)** | **%99.50** | **%88.24** |
| **Loss (Kayıp)** | `2.7420` | `2.9928` |

---

## 🛠️ Kullanılan Teknolojiler ve Kütüphaneler

* **Derin Öğrenme:** `TensorFlow (2.9.1)`, `Keras`
* **Görüntü İşleme:** `OpenCV (cv2)`, `Pillow (PIL)`, `ImageDataGenerator`
* **Veri Analizi ve Ön İşleme:** `Pandas`, `NumPy`, `Scikit-learn`
* **Görselleştirme:** `Matplotlib`, `Seaborn`

---

## 🚀 Kurulum ve Çalıştırma

Projeyi kendi bilgisayarınızda çalıştırmak için:

1. Depoyu klonlayın:
   ```bash
   git clone [https://github.com/azadaygun65-byte/brain-tumor-detection.git](https://github.com/azadaygun65-byte/brain-tumor-detection.git)
   cd brain-tumor-detection

   pip install -r requirements.txt

   jupyter notebook brain-tumor-detection.ipynb
