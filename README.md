# 🩺 Pneumonia Detection from Chest X-Ray Images using Deep Learning  

**Author:** Nari sai Karthikeya (IIT Kharagpur)  
📧 Email: [karthikeyanari19@gmail.com](mailto:karthikeyanari19@gmail.com)  
🔗 GitHub: [Karthikeya-ai-glitch](https://github.com/Karthikeya-ai-glitch)  
🔗 GitLab: [narikrthk](https://gitlab.com/narikrthk)  

---

## 📌 Project Overview  
This project applies **Deep Convolutional Neural Networks (CNNs)** and **Transfer Learning (InceptionV3)** to detect **Pneumonia** from chest X-ray images.  
The model classifies X-rays as **Normal** or **Pneumonia**, assisting doctors with faster and more reliable screening.  

---

## 📂 Dataset  
- **Dataset:** [Chest X-Ray Images (Pneumonia)](https://www.kaggle.com/paultimothymooney/chest-xray-pneumonia)  
- **Classes:**  
  - Normal  
  - Pneumonia  
- **Dataset Size:** ~5,856 images (~1.15 GB)  
  - Training: 5,216  
  - Validation: 320  
  - Testing: 320  

---

## 🛠️ Model & Techniques  
- **Custom CNN**  
  - Layers: Conv2D → MaxPooling → Dropout → Dense  
  - Optimizer: Adam, Loss: Binary Crossentropy  
  - Batch Size: 64, Epochs: 30  

- **Transfer Learning (InceptionV3)**  
  - Removed top layers, froze base layers, fine-tuned for binary classification  
  - Achieved comparable performance with higher generalization  

---

## 📊 Results  
- **Custom CNN:**  
  - Accuracy: **89.53%**  
  - Loss: **0.41**  
  - Precision: **88.37%**  
  - Recall (Pneumonia): **95.48%**  

📌 *Grad-CAM visualizations highlight infected lung regions, ensuring interpretability for medical decision-making.*  

---

## 📸 Sample Outputs  

**Prediction Example**  
<kbd>
<img src="demo/sample/sample.png">
</kbd>  

[See More Results](demo/images/result.png)  

**Confusion Matrix**  
<kbd>
<img src="demo/report/CM.png" width="800px" height="600px">
</kbd>  

---

## 🔧 Installation & Usage  

### 1️⃣ Clone the Repository  
```bash
git clone https://github.com/Karthikeya-ai-glitch/Pneumonia-Detection-Project.git
cd Pneumonia-Detection-Project
```

### 2️⃣ Install Dependencies  
```bash
pip install -r requirements.txt
```

### 3️⃣ Train the Model  
```bash
python train.py
```

### 4️⃣ Run Predictions  
```bash
python predict.py --image sample_xray.jpg
```

---

## 🛠️ Tools & Libraries  
- Python  
- TensorFlow / Keras  
- NumPy, Pandas  
- Matplotlib, Seaborn  
- OpenCV  
- Anaconda / Jupyter Notebook  

---

## 🏆 Key Takeaways  
✔️ Applied **Deep Learning & Transfer Learning** in healthcare AI  
✔️ Worked on **real-world medical imaging data**  
✔️ Integrated **Explainable AI (Grad-CAM)** for model transparency  

---

✨ *This project demonstrates how AI can assist healthcare professionals in early detection of pneumonia from chest X-ray images.*  
