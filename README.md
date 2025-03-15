# 🚀 AI-Powered Fraudulent Website Detector  

🔍 A browser extension that detects scam websites using AI (NLP, computer vision, and metadata analysis).  

## 🌟 Features  
✅ Detects phishing, fake e-commerce, and scam websites in real-time.  
✅ Uses AI to analyze website text, UI layout, and metadata.  
✅ Provides a **trust score (0-5 stars)** and an explanation for detection.  

## 📂 Project Structure  

fraud-website-detection/
│── backend/                  # Backend API & AI Models
│   ├── app.py                # Flask API for AI Model
│   ├── model/                # Folder for trained AI models
│   │   ├── scam_text_model.pth   # Trained NLP model (BERT)
│   │   ├── scam_ui_model.h5      # Trained CNN model (Website Layout)
│   ├── preprocess.py         # Data Preprocessing Script
│   ├── train_text_model.py   # Train NLP Scam Detector
│   ├── train_ui_model.py     # Train CNN Scam Detector
│   ├── requirements.txt      # Dependencies for backend
│── extension/                # Chrome Extension
│   ├── manifest.json         # Chrome Extension Configuration
│   ├── background.js         # Runs in the background (handles requests)
│   ├── content.js            # Extracts website data
│   ├── popup.html            # User Interface for the extension
│   ├── popup.js              # Handles UI interactions
│   ├── styles.css            # Styles for the popup
│── dataset/                  # Raw & Processed Data
│   ├── raw_data/             # Raw website text, screenshots, metadata
│   ├── processed_data.csv    # Preprocessed data ready for AI training
│── deployment/               # Deployment & Optimization
│   ├── deploy_api.py         # Deploys the Flask API to cloud
│   ├── optimize_model.py     # Converts AI model to ONNX for faster inference
│── README.md                 # Project Documentation



