# Cancer-Detector
We aim to provide a complete user experience with integrated medication and doctor-appointment APIs as well as awareness surrounding Skin cancer and allergies. Using 3 state-of-the-art Deep Learning Classification models we try to predict with considerably high accuracy if you are suffering from Melanoma (which is the most fatal type of skin cancer) or any other type of cancer (basal cell carcinoma, and  other types), or if you are suffering from an allergy (using a separate model). With features like, embedded videos, remedies, medicine browsing, Find a Doctor we hope to be a one-stop solution for the user's dermatological problems.

Models:
We have used 3 models for 3-layered multipurpose testing, namely, for detecting Melanoma(the most fatal type of Skin Cancer), the given types of Skin Cancers:
1.Basal Cell Carcinoma
2.Squamous Cell Crcinoma
3.Melanoma

Basically,the project is prepared using Teachable machine.

Training Overview:
The three models were trained on open source datasets, some using custom or transfer learning architectures on Kaggle Cloud GPUs. For specific training and model architecture refer to the training notebooks in Models/. The data pre-processing, scraping, augmentation techniques are also described in these notebooks. Models were trained using Tensorflow 2.0 deep learning framework, and were exported in .tflite (Tensorflow lite) format. For post-processing we have tested the models, then applied quantisation, pruning to clip inconsequential weights in the model an reduce it's size for deployment. The pre and post quantisation test results can be found in the model training notebooks as well.

Files in Repository:
Model Training, Data Preprocessing and Conversion to TFLite is shown in Skin-Cancer-Detection-App/Models/.. as Jupyter Notebooks. Data is taken from Kaggle for Melanoma Model and Cancer Model. For Allergy Model a custom scraper is implemented for obtaining data, which is shown in, Skin-Cancer-Detection-App/Models/allergy-model/..

Models in .tflite formats and their labels are in App/assets/

