# Image_Classification_With_Keras

# Projenin Ana Teması
Bu proje, TensorFlow arka uç olarak kullanarak Keras ile basit bir görüntü sınıflandırma modeli oluşturmayı göstermektedir. Model, giyim eşyalarının yer aldığı gri tonlamalı görüntülerden oluşan Fashion MNIST veri kümesi üzerinde eğitilmiştir. Bu projede kullanılan veri kümesi, 10 farklı giyim kategorisinden oluşan 70.000 gri tonlamalı görüntü içeren Fashion MNIST veri kümesidir. Veri kümesi eğitim, doğrulama ve test setleri olarak bölünmüştür.

# Kurulum
Bu projeyi çalıştırmak için bilgisayarınızda Python'un yüklü olması gerekmektedir. Gerekli kütüphaneleri yüklemek için pip kullanabilirsiniz:
pip install tensorflow matplotlib pandas

# Modelin Mimarisi
<ul>
  <li>Input Layer</li>
  <li>Flatten Layer</li>
  <li>300 nöronlu ve aktivasyon fonksiyonu ReLU olan Dense Layer (Hidden Layer 1)</li>
  <li>100 nöronlu ve aktivasyon fonksiyonu ReLU olan Dense Layer (Hidden Layer 2)</li>
  <li>10 nöronlu ve aktivasyon fonksiyonu softmax olan Output Layer</li>
</ul>

# Modelin Eğitimi
Model, eğitim setinden 5.000 örneklik bir doğrulama bölümü ile 30 epoch için eğitilmiştir. Kullanılan loss fonksiyonu "sparse categorical crossentropy"dir ve optimizer olarak "stochastic gradient descent (SGD)" seçilmiştir.

# Sonuçlar
Eğitim sonrası modelin performansı test seti üzerinde değerlendirilmiştir. Eğitim geçmişini (doğruluk ve kayıp) görselleştirmek için Matplotlib kullanılabilir.

----
----

# Main Theme of the Project
This project demonstrates how to build a simple image classification model with Keras using TensorFlow as a backend. The model is trained on the Fashion MNIST dataset of grayscale images of clothing items. The dataset used in this project is the Fashion MNIST dataset, which contains 70,000 grayscale images of 10 different clothing categories. The dataset is divided into training, validation and test sets.

Translated with DeepL.com (free version)
# Installation
You need to have Python installed on your computer to run this project. You can use pip to install the necessary libraries:
pip install tensorflow matplotlib pandas

# Architecture of the Model
<ul>
  <li>Input Layer</li>
  <li>Flatten Layer</li>
  <li>Dense layer with 300 neurons and ReLU activation (Hidden Layer 1)</li>
  <li>Dense layer with 100 neurons and ReLU activation (Hidden Layer 2)</li>
  <li>Output layer with 10 neurons and softmax activation</li>
</ul>

# Model's Training
The model is trained for 30 epochs with a validation section of 5,000 samples from the training set. The loss function used is “sparse categorical crossentropy” and “stochastic gradient descent (SGD)” was chosen as the optimizer.

# Results
After training, the performance of the model is evaluated on the test set. Matplotlib can be used to visualize the training history (accuracy and loss).
