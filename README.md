# 🧠 Skin Cancer Classification (Benign vs Malignant)

##  Overview

This project uses **Deep Learning (VGG19 Transfer Learning)** to classify skin lesions into:

* **Benign (Non-cancerous)**
* **Malignant (Cancerous)**

The model is trained on a balanced dataset of dermatoscopic images and achieves ~**79% accuracy**.



##  Dataset

* Total Images: **~1800**
* Image Size: **224 x 224**
* Classes: **Benign & Malignant**

Dataset source: Kaggle (Skin Cancer: Malignant vs Benign) 



##  Features

*  Transfer Learning using **VGG19**
*  Image Augmentation for better generalization
* Binary Classification (2 classes)
*  Model saving & prediction pipeline
*  Visualization of accuracy & loss


##  Model Architecture

* Base Model: **VGG19 (pre-trained on ImageNet)**
* Custom Layers:

  * Flatten
  * Dense (512, ReLU)
  * Dropout (0.5)
  * Dense (256, ReLU)
  * Dropout (0.5)
  * Output Layer (Softmax)


##  Installation

```bash
git clone https://github.com/pransh1/skin_cancer_classification.git
cd skin_cancer_classification
pip install -r requirements.txt
```

---

## ▶ How to Run

###  Train Model

Run the notebook:

```
Preprocess_classify_test.ipynb
```

### Run Predictions

```python
from keras.models import load_model
model = load_model('model_vgg19.h5')
```



##  Model Performance

* Accuracy: **~79.6%**
* Loss: ~0.43

---

##  Visualization

* Training vs Validation Accuracy
* Training vs Validation Loss


##  Future Improvements

*  Improve accuracy using ResNet / EfficientNet
*  Deploy using Streamlit Cloud
*  Add real-time image upload UI
*  Hyperparameter tuning



##  Contributors

* Shivansh Rana 2210990831
* Priyanshu Sani 2210990688
* Pransh Maurya 2210990668
* Sulabh Garg 2210990871

##  Disclaimer

This project is for **educational purposes only** and should not be used for real medical diagnosis.
