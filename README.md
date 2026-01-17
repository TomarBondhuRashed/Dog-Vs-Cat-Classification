# 🐶 Dog vs. Cat Classifier (MobileNetV2)

### 🚀 Day 15 of 30: Machine Learning Projects Challenge

**Goal:** Build a Computer Vision model capable of distinguishing between dogs and cats with high accuracy.
**The Approach:** Transfer Learning using **MobileNetV2** (pre-trained on ImageNet).
**Dataset : https://www.kaggle.com/datasets/bhavikjikadara/dog-and-cat-classification-dataset**

---

## 🧐 The Challenge: "The Bleeding Edge Breaks"
I initially attempted this project using **Python 3.14**, only to discover that **TensorFlow** does not yet support it.
* **Attempt 1:** Built a basic classifier using **Scikit-Learn** (SVM) on Python 3.14. It worked but lacked deep learning accuracy.
* **Attempt 2 (The Fix):** Downgraded to **Python 3.10.11** to unlock the full power of TensorFlow/Keras.
* **Result:** Successfully implemented **MobileNetV2**, a state-of-the-art pre-trained model, achieving significantly higher accuracy than the scratch model.

---

## 🛠️ Tech Stack
* **Python 3.10.11** (Stable Environment)
* **TensorFlow / Keras** (Deep Learning)
* **MobileNetV2** (Pre-trained Model for Transfer Learning)
* **OpenCV & Pillow** (Image Processing)
* **Matplotlib** (Visualization)

---

## 🧠 Model Architecture
Instead of training a CNN from scratch (which takes hours and millions of images), I used **Transfer Learning**:
1.  **Base Model:** MobileNetV2 (Pre-trained on 1.4M images from ImageNet).
2.  **Frozen Layers:** I froze the base layers to keep the pre-learned patterns (edges, textures).
3.  **Custom Head:** Added a Global Average Pooling layer and a final Dense output layer for binary classification (Dog vs. Cat).

---

## 📝 How to Run
1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/TomarBondhuRashed/dog-vs-cat-classifier.git](https://github.com/TomarBondhuRashed/dog-vs-cat-classifier.git)
    ```
2.  **Set up the Environment (Crucial!):**
    Ensure you are using Python 3.8 - 3.11.
    ```bash
    conda create -n tf_env python=3.10
    conda activate tf_env
    pip install tensorflow numpy matplotlib opencv-python
    ```
3.  **Run the Notebook:**
    Open `Dog_vs_Cat_MobileNetV2.ipynb`.

---

## 🤝 Connect
Follow my 30-day coding journey!
* **LinkedIn:** [Your Profile Link]
* **GitHub:** [TomarBondhuRashed](https://github.com/TomarBondhuRashed)
