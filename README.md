# Brain Tumor Classification Using Deep Learning

Bu repo, Kaggle ortamında GPU (Tesla P100) kullanılarak **MRI görüntülerinden beyin tümör sınıflandırması** yapmak için geliştirilmiştir. Proje, Global AI Hub Bootcamp kapsamında hazırlanmıştır.

---

## Giriş
Bu projede [Brain Tumor MRI Dataset](https://www.kaggle.com/datasets/masoudnickparvar/brain-tumor-mri-dataset) kullanılmıştır.  

Çalışma sürecinde:  
- **Veri önişleme** (boyutlandırma, normalize etme, augmentation)  
- **CNN tabanlı bir model oluşturma**  
- **Transfer Learning (VGG16)** yaklaşımı  
- **Hiperparametre optimizasyonu (Keras Tuner)**  
- **Model değerlendirmesi (Accuracy/Loss grafikleri, Confusion Matrix, Grad-CAM)**  

adımları uygulanmıştır.  

Notebook içerisinde, her kod hücresine eklenen Markdown açıklamaları ile projenin teknik detayları açıklanmıştır.  

---

## Metrikler
Elde edilen en iyi sonuçlar:  
- **Eğitim doğruluğu:** %97.7  
- **Doğrulama doğruluğu:** %95.4  
- **Test doğruluğu:** ≈ %95  

**Yorum:**  
- Model, “No Tumor” ve “Pituitary” sınıflarında neredeyse kusursuz sonuç verirken, **Glioma** ve **Meningioma** sınıflarında zaman zaman karışmalar gözlenmiştir.  
- Grad-CAM görselleştirmeleri, modelin tahmin yaparken tümör bölgelerine odaklandığını göstermektedir.  
- Hiperparametre optimizasyonu (dropout, dense units, optimizer, learning rate) modelin daha dengeli hale gelmesini sağlamıştır.  

---

## Ekler
Bu projede ayrıca:  
- **Data Augmentation** ile modelin genelleme gücü artırılmıştır.  
- **TensorBoard** ile modelin eğitimi takip edilebilecek şekilde hazırlanmıştır.  

Gelecekte proje genişletilerek:  
- **Streamlit veya Gradio** tabanlı bir arayüz eklenebilir.  
- Gerçek zamanlı veri ile (örn. MR cihazlarından gelen) uçtan uca çalışacak bir pipeline kurulabilir.  
- Daha farklı transfer learning modelleri (ResNet, EfficientNet) ile karşılaştırmalar yapılabilir.  

---

## Sonuç ve Gelecek Çalışmalar
Bu proje, beyin tümörlerinin MRI görüntülerinden otomatik sınıflandırılmasının mümkün olduğunu göstermiştir.  
%95 üzeri doğruluk elde edilmiş olup, bu tür projeler doktorlara **tanı destek sistemi** olarak yardımcı olabilir.  

Gelecek çalışmalar için:  
- Daha büyük ve çeşitlendirilmiş veri setleri ile model geliştirilebilir.  
- Modelin mobil veya web tabanlı uygulamalara entegrasyonu sağlanabilir.  
- Gerçek zamanlı tıbbi sistemlerde kullanılmak üzere optimize edilebilir.  

---

## Linkler
- **Kaggle Notebook Linki:** [Kaggle Çalışmam]([https://www.kaggle.com/](https://www.kaggle.com/code/sudetacer/notebook2ae338eafe))  
- **Dataset Linki:** [Brain Tumor MRI Dataset](https://www.kaggle.com/datasets/masoudnickparvar/brain-tumor-mri-dataset)  
