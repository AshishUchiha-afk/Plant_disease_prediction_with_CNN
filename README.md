# Plant_disease_prediction_with_CNN
A CNN-based model to predict plant diseases from leaf images using deep learning with TensorFlow and Keras.

## ⚠️ Note on Model File Size & GitHub Limitations

Due to GitHub's file upload limit of **100 MB**, the trained CNN model (`plant_disease_prediction_model.h5`) — which is approximately **500 MB** — cannot be stored directly in this repository.

### 📥 How to Use the Model Locally

To keep the project accessible and reproducible:

1. **A placeholder link** to download the `.h5` model file from **Google Drive** is included in the `trained_model/` folder.
2. Run the script in **app.py**.
3. This allows you to run the **Streamlit app locally** without manually placing the model file.

> 🔁 If you prefer, you can also manually download the `.h5` model from the provided Drive link and place it inside the `trained_model/` folder before running the app.

---

### 🚀 To Run the App Locally

```bash
pip install -r requirements.txt
streamlit run app.py

---


## ⚙️ How to Run the Code Without Hassle in google colab

Follow the steps below to get started easily:

1. 📥 **Run the following cell in the notebook:**

   ```python
   from google.colab import files
   files.upload()
2.🔐 Upload your Kaggle token (kaggle.json) when prompted.

3.✅ Now the code is ready to run — all necessary permissions and access will be set up!

## ⚙️ How to Set Up the Project Locally (Kaggle API Method)

Follow these steps if you want to use the Kaggle API to download the dataset directly:

1. 🔑 **Get Your Kaggle API Credentials**  
   - Go to your [Kaggle Account Settings](https://www.kaggle.com/account)
   - Click on **"Create New API Token"**
   - This will download a file called `kaggle.json`

2. 📁 **Place the Token File**  
   - Move `kaggle.json` to the `.kaggle` folder:
     - On Windows: `C:\Users\<YourUsername>\.kaggle\kaggle.json`
     - On macOS/Linux: `~/.kaggle/kaggle.json`

3. 🧠 **Use the Following Code to Programmatically Download the Dataset**

   ```python
   import os
   import kaggle

   # Set Kaggle credentials (optional if kaggle.json is correctly placed)
   os.environ['KAGGLE_USERNAME'] = 'your_username'
   os.environ['KAGGLE_KEY'] = 'your_key'

   # Download and unzip the dataset
   kaggle.api.dataset_download_files('dataset', path='.', unzip=True)


# 🌿 Plant Disease Prediction using Convolutional Neural Networks (CNN)

This project uses a Convolutional Neural Network (CNN) to identify and classify plant diseases from leaf images. The goal is to assist farmers and agricultural professionals in early detection of crop diseases using AI-powered image classification.

## 🧠 Project Highlights

- ✅ Built using TensorFlow and Keras
- 🖼️ Trained on labeled images of healthy and diseased leaves
- 📊 Achieves high accuracy on test data
- 📦 Data preprocessing includes image resizing, normalization, and augmentation
- 🧪 Includes train-test-validation split and model evaluation
- 📈 Plots for accuracy, loss, and model performance included


## 🛠️ Technologies Used

- Python
- TensorFlow / Keras
- NumPy / Matplotlib
- OpenCV (optional for image preprocessing)

## 📌 How It Works

1. Image dataset is preprocessed and augmented.
2. A CNN model is built and trained on the training set.
3. Model performance is validated using validation data.
4. Test images are evaluated, and predictions are made.

## 📷 Sample Output

> ![image](https://github.com/user-attachments/assets/0fd7ecc6-798e-4d52-8332-88ba49dca166)
> 


## 🚀 Future Improvements

- Add more plant types and diseases
- Improve accuracy using transfer learning (e.g., MobileNet, EfficientNet)

---

Feel free to fork, improve, or integrate this into your own projects!


