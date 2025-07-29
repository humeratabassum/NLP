**Case Study: Spam Email Detection Using NLP Pipeline**

A basic machine learning pipeline to classify emails as **Spam** or **Not Spam** using text processing and classification techniques.


<img width="793" height="655" alt="Screenshot (6)" src="https://github.com/user-attachments/assets/6aaa4235-ac0c-4bc2-9c78-79f534b78657" />

## 🧾 Pipeline Overview

### 1. Data Collection
- Gathered a labeled dataset of emails.
- Example sources:
  - Enron Email Dataset
  - UCI Spam Dataset

---

### 2. Text Cleaning
- Removed:
  - HTML tags
  - Special characters
  - URLs
  - Numbers
  - Extra white spaces
- Converted all text to lowercase for consistency.

---

### 3. Pre-processing
- **Tokenization**: Split text into individual words.
- **Stopword Removal**: Removed common words (e.g., “the”, “is”, “in”).
- **Stemming / Lemmatization**: Reduced words to their root forms  
  (e.g., "running" → "run").

---

### 4. Feature Engineering
Converted processed text into numerical features using:
- **Bag of Words (BoW)**
- **TF-IDF (Term Frequency-Inverse Document Frequency)**

---

### 5. Modeling
Trained classification models using the extracted features:
- Logistic Regression
- Naive Bayes

---

### 6. Evaluation
Evaluated model performance on a test set using:
- **Accuracy**
- **Precision**
- **Recall**
- **F1-Score**

---

### 7. Deployment
- Integrated the trained model as an API or into an email client.
- Filters incoming emails in real-time.

---

### 8. Monitoring and Model Updating
- Tracked:
  - False positives (ham classified as spam)
  - False negatives (spam classified as ham)
- Periodically updated the model with new data for improved performance.
