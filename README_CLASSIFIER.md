# 🐱🐶 IMAGE CLASSIFIER - Cat & Dog

## 📌 Project Overview
This project is an **image classification system** designed to distinguish between **cats 🐱 and dogs 🐶** using a **Convolutional Neural Network (CNN)** based on the **VGG16** architecture.

The model was trained on a **25,000-image dataset** from Kaggle’s **Dogs vs. Cats** competition. The project serves as a **prototype**, with future expansions planned for a **web application**.

---

## 📊 Model Performance

| Metric            | Training Set | Validation Set |
|------------------|-------------|---------------|
| **Accuracy**     | **91.28%**   | **90.78%**    |
| **Loss**         | **0.1991**   | **0.2140**    |

✅ The model achieved **high accuracy** with minimal overfitting.

---

## 🚀 How It Works
### **1️⃣ Data Preprocessing**
- **Images resized to 200x200 pixels** for efficiency.  
- **Data Augmentation** applied for improved generalization.  
- **80/20 split** between training and validation sets.

### **2️⃣ Model Architecture**
- Used **VGG16 pre-trained model** as a feature extractor.  
- Added **custom dense layers** for binary classification.  
- Optimized with **Adam optimizer** and **binary crossentropy loss**.

### **3️⃣ Training & Optimization**
- Trained for **10 epochs** using **data augmentation**.  
- Implemented **ModelCheckpoint** to save the best model.  
- **EarlyStopping** used to prevent overfitting.

### **4️⃣ Predictions**
- The model can classify **single images** as **Cat or Dog** with high confidence.

---

## 📁 Why We Did NOT Include the Model File (`.keras`)
The trained model (`best_model.keras`) **is not included** in this repository because:
1. **Size Constraints** 📏 → The model is **1.09 GB**, making it impractical for GitHub.
2. **Better Alternatives** 🔗 → Instead, you can **retrain the model** using this repository.
3. **Future Deployment** 🌍 → The model will be hosted online in a **web app**.

⚡ **Want the trained model?** You can generate it by running:
```python
best_model.save("best_model.keras")
