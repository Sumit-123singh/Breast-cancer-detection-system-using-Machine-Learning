🧠 Breast Cancer Prediction - FastAPI App

This project is a machine learning deployment using FastAPI for breast cancer prediction. It takes medical feature inputs from a web form and predicts whether the tumor is Malignant (Cancer) or Benign (Not Cancer).

🚀 Live Demo (Optional)

🔗 View Live App(Replace with your actual deployed link)

📦 Clone This Repository

git clone https://github.com/Sumit-123singh/Breast-cancer-detection-system-using-Machine-Learning

💧 Project Structure

ml_flask_deploy/
├── app.py                         # FastAPI main app
├── model.pkl                      # Trained ML model
├── requirements.txt               # Python dependencies
├── .gitignore                     # Files to ignore in Git
├── README.md                      # Documentation

├── templates/
│   └── index.html                 # Frontend form

├── static/
│   └── images/
│       ├── alert_image.png
│       ├── img.jpg
│       └── okay_img.jpg

├── anaconda_projects/
│   ├── breast_cancer_prediction_model.ipynb  # Model training notebook
│   └── breast cancer.csv                     # Dataset

⚙️ Environment Setup

Python 3.10 or above is recommended

Create a virtual environment:

python -m venv venv
source venv/bin/activate    # On Windows: venv\Scripts\activate

Install dependencies:

pip install -r requirements.txt

🚀 Run the App Locally

uvicorn app:app --reload

Visit: http://127.0.0.1:8000

Swagger Docs: http://127.0.0.1:8000/docs

🧠 ML Model Details

Model Type: Logistic Regression Classifier (or similar)

Dataset: breast cancer.csv (UCI repository or scikit-learn)

🌐 Deployment (Render)

Add Build Command:

pip install -r requirements.txt

Start Command:

gunicorn app:app

Environment Variables (on Render dashboard):

SECRET_KEY=generated throgh vs code terminal using command "python -c "import secrets; print(secrets.token_urlsafe(32))"
FLASK_ENV=production
MODEL_PATH=model.pkl

Ensure gunicorn is in requirements.txt








👨‍💻 Author

Sumit Singh
ML Enthusiast| Backend Developer
