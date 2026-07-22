# 📧 Email Spam Classifier

A Machine Learning project that classifies emails as **Spam** or **Ham (Not Spam)** using Natural Language Processing (NLP) and Scikit-learn. This project demonstrates the complete ML pipeline from data preprocessing to model deployment.

---

## 🚀 Features

- 📩 Detects whether an email is Spam or Ham
- 📝 Text preprocessing using NLP
- 🔤 Tokenization
- 🔡 Lowercase conversion
- 🚫 Stopword removal
- 🌱 Stemming
- 📊 TF-IDF Vectorization
- 🤖 Machine Learning Model Training
- 💾 Save trained model using Joblib
- ⚡ Fast and accurate predictions

---

## 🛠️ Tech Stack

- Python 3
- Pandas
- NumPy
- Scikit-learn
- NLTK
- Joblib
- Matplotlib
- Seaborn (Optional)

---

## 📂 Project Structure

```
Email-Spam-Classifier/
│
├── dataset/
│   └── spam.csv
│
├── notebooks/
│   └── Email_Spam_Classifier.ipynb
│
├── saved_models/
│   ├── model.pkl
│   ├── vectorizer.pkl
│   └── transformer.pkl
│
├── app.py
├── train.py
├── predict.py
├── requirements.txt
├── README.md
└── LICENSE
```

---

## 📊 Dataset

The project uses the **SMS Spam Collection Dataset**.

Dataset contains:

- **Spam** messages
- **Ham (Not Spam)** messages

Typical columns:

| Column | Description |
|---------|-------------|
| label | Spam or Ham |
| message | Email/SMS text |

---

## ⚙️ Installation

Clone the repository:

```bash
git clone https://github.com/your-username/Email-Spam-Classifier.git
```

Move into the project:

```bash
cd Email-Spam-Classifier
```

Create a virtual environment:

### Linux / macOS

```bash
python3 -m venv venv
source venv/bin/activate
```

### Windows

```bash
python -m venv venv
venv\Scripts\activate
```

Install dependencies:

```bash
pip install -r requirements.txt
```

---

## ▶️ Training the Model

Run:

```bash
python train.py
```

This will:

- Load dataset
- Clean text
- Perform NLP preprocessing
- Convert text into TF-IDF vectors
- Train the classifier
- Save the trained model

---

## 🧹 Text Preprocessing

The preprocessing pipeline includes:

- Convert text to lowercase
- Remove punctuation
- Tokenization
- Remove stopwords
- Stemming using PorterStemmer

Example:

Input:

```
Congratulations!! You won $1000.
Click here now!!!
```

Processed:

```
congratul won click
```

---

## 🤖 Machine Learning Pipeline

```
Raw Email
      │
      ▼
Text Cleaning
      │
      ▼
Tokenization
      │
      ▼
Stopword Removal
      │
      ▼
Stemming
      │
      ▼
TF-IDF Vectorizer
      │
      ▼
Machine Learning Model
      │
      ▼
Prediction
```

---

## 📈 Model Evaluation

Common evaluation metrics:

- Accuracy
- Precision
- Recall
- F1 Score
- Confusion Matrix

Example:

```
Accuracy : 98%

Precision : 99%

Recall : 97%

F1 Score : 98%
```

---

## 🔍 Predicting New Emails

Example:

```python
email = "Congratulations! You have won a free iPhone."

prediction = model.predict(vectorizer.transform([email]))

print(prediction)
```

Output:

```
Spam
```

---

## 📦 Saved Models

The trained models are stored in:

```
saved_models/
```

Example files:

```
model.pkl
vectorizer.pkl
transformer.pkl
```

---

## 📸 Screenshots

Add screenshots here after building the application.

Example:

```
screenshots/
│
├── home.png
├── prediction.png
└── result.png
```

---

## 📚 Future Improvements

- 🌐 Web interface using FastAPI or Flask
- ⚛️ React frontend
- ☁️ Cloud deployment
- 📧 Real email integration
- 🔍 Deep Learning (LSTM/BERT)
- 📱 Mobile application

---

## 🤝 Contributing

Contributions are welcome!

1. Fork the repository
2. Create a new branch

```bash
git checkout -b feature-name
```

3. Commit changes

```bash
git commit -m "Added new feature"
```

4. Push

```bash
git push origin feature-name
```

5. Open a Pull Request

---

## 📄 License

This project is licensed under the MIT License.

---

## 👨‍💻 Author

**Sarthak Adhikari**

- 💻 Passionate about Machine Learning and AI
- 🚀 Learning Deep Learning and Full Stack Development
- 🌍 Interested in solving real-world problems using Artificial Intelligence

---

## ⭐ Support

If you found this project helpful:

⭐ Star the repository

🍴 Fork the project

🛠️ Contribute to improve it

---

> Built with ❤️ using Python, NLP, and Machine Learning.