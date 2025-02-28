# TurkceDuyguAnalizi
Bu çalışma, müşteri incelemelerini analiz ederek işletmelere içgörü sağlamak amacıyla geliştirilmiştir. Pandas ve NumPy kullanılarak veri işleme, TensorFlow ve Keras ile GRU tabanlı derin öğrenme modeli eğitilmiş, Flask API ile entegrasyon sağlanmıştır. Model sonuçları yeşil (pozitif), kırmızı (negatif) ve gri (nötr) renklerle görselleştirilmiştir.
Tam metne ve makaleye ulaşmak için https://www.linkedin.com/pulse/bitirme-tezim-yay%C4%B1nda-hayrettin-dal-koccf/?trackingId=kVlUSOhqQ6SaOm%2FQUS6pcw%3D%3D

# Sentiment Analysis of E-Commerce Reviews

## 📌 Project Overview
This project performs **Sentiment Analysis** on customer reviews collected from various **e-commerce platforms**. It utilizes **Natural Language Processing (NLP)** and **Deep Learning** techniques to classify reviews as **positive, negative, or neutral**. The model is deployed using a **Flask API** for real-world applications.

## 🚀 Features
- **Data Processing:** Cleans and preprocesses text data using `pandas` and `NumPy`.
- **Deep Learning Model:** Uses a **GRU-based neural network** built with `TensorFlow` and `Keras`.
- **Sentiment Classification:** Predicts sentiments as **positive, negative, or neutral**.
- **API Deployment:** Flask-based REST API for model inference.
- **User-Friendly Interface:** Results are displayed in green (positive), red (negative), and gray (neutral).

## 🏗️ Tech Stack
- **Programming Language:** Python
- **Frameworks & Libraries:**
  - `TensorFlow` & `Keras` (Deep Learning)
  - `pandas` & `NumPy` (Data Processing)
  - `Flask` (API Deployment)
  - `Jupyter Notebook` (Development)
  - `Bootstrap` (Frontend UI)
- **Database:** CSV files for training & inference

## 📂 Project Structure
```
├── data/                 # Dataset for training & evaluation
├── model/                # Trained model files
├── api/
│   ├── app.py            # Flask API for model inference
│   ├── requirements.txt  # Dependencies
│   ├── templates/
│   ├── static/
├── notebooks/            # Jupyter Notebooks for model training & evaluation
├── README.md             # Project documentation
```

## ⚙️ Installation & Setup
```bash
# Clone the repository
git clone https://github.com/yourusername/sentiment-analysis-nlp.git
cd sentiment-analysis-nlp

# Create a virtual environment
python -m venv venv
source venv/bin/activate  # On Windows use `venv\Scripts\activate`

# Install dependencies
pip install -r api/requirements.txt
```

## 🏃 Running the Application
```bash
# Start the Flask API
cd api
python app.py
```
Now, open your browser and navigate to `http://127.0.0.1:5000/` to access the web interface.

## 📊 Model Training
If you want to train the model from scratch:
```bash
cd notebooks
jupyter notebook
```
Run `train_model.ipynb` to preprocess data and train the GRU-based deep learning model.

## 🔥 Example API Request
To test the API using `curl`:
```bash
curl -X POST http://127.0.0.1:5000/predict -H "Content-Type: application/json" \
  -d '{"review": "This product is amazing!"}'
```
**Response:**
```json
{
  "sentiment": "positive",
  "confidence": 0.92
}
```

## 📌 Future Enhancements
- Expanding dataset for better accuracy.
- Implementing real-time analysis with streaming data.
- Deploying as a cloud-based service.

## 📝 License
This project is licensed under the **MIT License**.

## 👨‍💻 Author
**Hayrettin Dal**  
[GitHub](https://github.com/hayro45) | [LinkedIn](https://www.linkedin.com/in/hayrettin-dal-94028a182/)
