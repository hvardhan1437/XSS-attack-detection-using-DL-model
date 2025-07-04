# Cross site scripting (XSS) detection using DL model 🚀

A hybrid deep learning + rule-based system to detect Cross-Site Scripting (XSS) attacks in real time using a Bidirectional LSTM (BiLSTM) neural network and regex patterns. Built with FastAPI backend and an interactive HTML frontend.

## 📌 Project Overview
This mini-project is a secure, fast, and explainable XSS attack detection system that:

- Leverages a BiLSTM model trained on 13,686 labeled HTML/script snippets.
  
- Combines deep learning with rule-based regex filters to identify both known and novel attack patterns.
  
- Delivers real-time predictions with confidence scores via a sleek web interface built with HTML/CSS/JS.
  
- Uses FastAPI as a high-performance backend for serving predictions.


## 📈 Highlights

- ✅ Accuracy: 99.71% test accuracy

- ⚡ Fast Inference: Optimized backend with model preloading

- 🔍 Explainability: Shows pattern-based reasons for XSS detection

- 🧠 BiLSTM Power: Captures both past and future context in sequences

- 💻 Responsive UI: Modern frontend with animated confidence bars


## 🛠️ Tech Stack
- Backend: Python, FastAPI, TensorFlow, Keras, Uvicorn

- Frontend: HTML, CSS, JavaScript

- Libraries: NumPy, Pandas, scikit-learn, Matplotlib

- Model: BiLSTM with Embedding → BiLSTM → Dense + Dropout

- Dataset link: [https://www.kaggle.com/datasets/syedsaqlainhussain/cross-site-scripting-xss- dataset-for-deep-learning](https://www.kaggle.com/datasets/syedsaqlainhussain/cross-site-scripting-xss-dataset-for-deep-learning)


## 🔬 How it works
1. User Input: HTML/script content is entered via web UI.

2. Preprocessing: Tokenized and padded using Keras.

3. Rule-Based Check: Regex patterns detect known attack forms.

4. ML Prediction: BiLSTM evaluates contextual intent of input.

5. Result: User sees "XSS Detected" or "Safe" with confidence.


## 🔮 Future Enhancements
The current system was trained on a dataset of approximately 13,686 labeled samples, which, while effective, may limit the generalization of the model in real-world scenarios. Future improvements could include:

- Dataset Expansion: Acquiring a larger and more diverse dataset, especially with real-world, obfuscated, and DOM-based XSS payloads, can significantly enhance the model's performance. More data would allow exploration of:

  * Rare or zero-day XSS attack patterns

  * Advanced adversarial examples

  * Better handling of multilingual or encoded content

- Transformer-Based Models: With a larger dataset, powerful architectures like BERT, RoBERTa, or other Transformers can be fine-tuned for deeper semantic understanding, improving detection in complex input scenarios.

- Improved Obfuscation Detection: Many XSS payloads use encoding or script obfuscation to bypass filters. Future work can incorporate:

     * HTML/JS decoding layers

     * Canonicalization to normalize inputs before detection

- Production-Ready Features:

     * API authentication to secure endpoints

     *Logging and monitoring to track usage and attacks

     * Rate limiting to prevent misuse or abuse

- Scalable Deployment: Containerize and deploy the app using services like Docker, Heroku, AWS, or Google Cloud Platform for broader real-time access and load handling.

- Continuous Learning Pipeline: As new XSS samples are encountered, an active learning framework can be integrated for automatic retraining and model updates over time.


## XSS Attack  Flowchart

![image](https://github.com/user-attachments/assets/cfab94fa-bca4-43eb-ba34-0669f0cd023d)

## Block Diagram of BiLSTM Model

![image](https://github.com/user-attachments/assets/8dc88346-4f0b-4e8f-990d-cff3702e1a47)

## Results of the BiLSTM  model

 - Model Accuracy vs Model Loss

 ![image](https://github.com/user-attachments/assets/69bd1691-3f28-4c9f-b241-c0cdd4ba13a8)

 - Test Accuracy

   ![image](https://github.com/user-attachments/assets/02af4224-dfd6-4320-866d-6d3d458f768f)

 - Classification Report

 ![image](https://github.com/user-attachments/assets/60ba36cd-2ec5-41a7-8581-d894871356ba)


## User Interface

![image](https://github.com/user-attachments/assets/324cff65-f99f-4e7e-9146-7ba032063b54)


## ✨ Team Members


    Alajangi Venkata Satya .
    K N Lakshmi .
    K Hemavardhan Reddy .
    K V Vamshidhar Reddy .
    DR. Pradeep Menon .
  



