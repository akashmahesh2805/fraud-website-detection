# 🚀 AI-Powered Fraudulent Website Detector  

🔍 A browser extension that detects scam websites using AI (NLP, computer vision, and metadata analysis).  

## 🌟 Features  

✅ Detects phishing, fake e-commerce, and scam websites in real-time.  
✅ Uses AI to analyze website text, UI layout, and metadata.  
✅ Provides a **trust score (0-5 stars)** and an explanation for detection.  

## 📂 Project Structure  

fraud-website-detection/<br/>
│── backend/                  # Backend API & AI Models<br/>
│   ├── app.py                # Flask API for AI Model<br/>
│   ├── model/                # Folder for trained AI models<br/>
│   │   ├── scam_text_model.pth   # Trained NLP model (BERT)<br/>
│   │   ├── scam_ui_model.h5      # Trained CNN model (Website Layout)<br/>
│   ├── preprocess.py         # Data Preprocessing Script<br/>
│   ├── train_text_model.py   # Train NLP Scam Detector<br/>
│   ├── train_ui_model.py     # Train CNN Scam Detector<br/>
│   ├── requirements.txt      # Dependencies for backend<br/>
│── extension/                # Chrome Extension<br/>
│   ├── manifest.json         # Chrome Extension Configuration<br/>
│   ├── background.js         # Runs in the background (handles requests)<br/>
│   ├── content.js            # Extracts website data<br/>
│   ├── popup.html            # User Interface for the extension<br/>
│   ├── popup.js              # Handles UI interactions<br/>
│   ├── styles.css            # Styles for the popup<br/>
│── dataset/                  # Raw & Processed Data<br/>
│   ├── raw_data/             # Raw website text, screenshots, metadata<br/>
│   ├── processed_data.csv    # Preprocessed data ready for AI training<br/>
│── deployment/               # Deployment & Optimization<br/>
│   ├── deploy_api.py         # Deploys the Flask API to cloud<br/>
│   ├── optimize_model.py     # Converts AI model to ONNX for faster inference<br/>
│── README.md                 # Project Documentation<br/>



