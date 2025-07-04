# 👁️ OCT Retinal Disease Classification

## 🎯 Objective
Building a deep learning model to classify **OCT retina images** into:
- CNV
- DME
- DRUSEN
- NORMAL

to assist in early detection of retinal diseases.

## 🛠️ Tech Stack
- Python
- TensorFlow / Keras
- Matplotlib, Pandas, Numpy

## 📊 Results
 Achieved **95% accuracy** on the test set.  
 Visualized predictions on sample OCT images.  
 Trained using CNN with data augmentation.

## 📂 Dataset
We used the **[OCT Retina (Kermany) dataset](https://www.kaggle.com/datasets/paultimothymooney/kermany2018)** containing **retinal OCT images** classified into:
- **CNV** (Choroidal Neovascularization)
- **DME** (Diabetic Macular Edema)
- **DRUSEN**
- **NORMAL**

### Dataset Details:
 Contains **over 84,000 labeled OCT images** for training and validation.  
 Images are in JPEG format with varying resolutions.  
 Each class is stored in a **separate folder**:
\`\`\`
/OCT/
   ├── CNV/
   ├── DME/
   ├── DRUSEN/
   └── NORMAL/
\`\`\`
The dataset represents **real clinical cases**, helping the model learn **clinically relevant patterns** for practical deployment.

### Sample Images:
- CNV: shows fluid beneath the retina.
- DME: exhibits retinal thickening.
- DRUSEN: yellow deposits under the retina.
- NORMAL: healthy retinal layers.

### Data Augmentation:
To improve generalization, we applied:
- Random rotations
- Horizontal flips
- Zoom and shift

This helped **mitigate overfitting** and handle class imbalance effectively.

## 📈 Future Improvements
- Hyperparameter tuning to further improve accuracy.
- Model quantization for mobile deployment.
- Integration with Streamlit for web-based prediction.
