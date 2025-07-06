## How to Run the Script
#  Image Classification using Teachable Machine & Keras

This project demonstrates how to train a custom image classification model using [Teachable Machine by Google](https://teachablemachine.withgoogle.com/) and use it with Python to make predictions on new images.

---

##  Project Steps

### 1. Model Training
- Trained using Teachable Machine
- Includes 2 classes (e.g., Cats and Dogs)
- Exported in TensorFlow → Keras (.h5) format
- Files downloaded:
  - keras_model.h5
  - labels.txt

---

### 2. Python Prediction Script

A Python script (`predict.py`) was written to:
- Load the trained .h5 model
- Preprocess an input image to the correct format
- Predict the image class using the model
- Display the class name and confidence score

---

### 3. Files Included

| File               | Description                          |
|--------------------|--------------------------------------|
| predict.py       | Python script for loading the model and predicting |
| keras_model.h5   | Trained model file exported from Teachable Machine |
| labels.txt       | Text file containing class labels    |
| screenshot.png   | Screenshot of the prediction output  |
| test_image.jpg   | Sample image used for testing (optional) |

---
1. Install dependencies:
```bash
! pip install tensorflow==2.12.1

2. Place your test image in the same folder as the script.

3. Edit the image path in the script if needed, for example:
image = Image.open("cat.jpg").convert("RGB")

4.Run the script:
python predict.py

Sample output

• Class: cat
 • Confidence Score: 0.987

 Notes
 • Make sure all files (.h5, labels.txt, and image) are in the correct path.
 • This project is for educational purposes and demonstrates how machine learning can be applied in a simple and intuitive way using Teachable Machine + Keras.

 Credits
 • Model trained using Teachable Machine
 • Script written and tested using Python 3 + TensorFlow 2.12
