
Automatic Essay Scoring System - NLP Final Project
==================================================

📚 Project Description:
-----------------------
This project presents an intelligent system for Automatic Essay Scoring (AES) using Natural Language Processing (NLP) and machine learning. The system is capable of reading student-written essays and predicting their quality score. It uses both traditional ML approaches and transformer-based models to learn from real human-scored data.

🎯 Objective:
-------------
To build a robust and explainable essay scoring model that can predict human-like scores for essays from the ASAP dataset. This helps in reducing grading time, maintaining consistency, and enabling scalable evaluation for educational platforms.

🛠️ Methods & Models:
---------------------
We experimented with multiple modeling strategies:
1. Random Forest with TF-IDF and handcrafted features  
2. Sentence-BERT embeddings combined with spelling & grammar features  
3. Fine-tuned DistilBERT Regressor (v3/v4)  
Each version was compared using MAE, RMSE, R², and Pearson Correlation.

📊 Final Model Performance:
---------------------------
- ✅ MAE: 0.53
- ✅ RMSE: 0.70
- ✅ R² Score: 0.68
- ✅ Pearson Correlation: 0.83  
This indicates a highly reliable model suitable for real-world automated scoring tasks.

📁 Folder Structure:
--------------------
Essay-Grading-NLP-Project/
│
├── Final_Project.ipynb              → Main notebook (training & evaluation)
├── README.txt                       → This file
├── requirements.txt                 → Python dependencies
│
├── essay_tokenizer/                → Saved tokenizer files
├── model/
│   └── essay_grader_model.pt       → Final trained model
│
└── data/
    └── essays_for_finetuning.csv   → Cleaned training dataset

📦 Dataset Reference:
---------------------
This project uses the ASAP Automated Essay Scoring Dataset by The Hewlett Foundation.  
Available here: https://www.kaggle.com/datasets/currie32/asap-aes

💡 Notes:
---------
- The model predicts continuous essay scores (e.g., 1.0–12.0), not grade letters (A–F).
- Preprocessing includes: text cleaning, spelling/grammar detection, and embedding extraction.
- All experiments were executed and tested in VS Code

👨‍💻 Author:
------------
Developed as part of the Natural Language Processing course final project by an AI student at the Arab Academy for Science and Technology.
