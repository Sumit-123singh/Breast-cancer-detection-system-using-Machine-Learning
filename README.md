🧠 Breast Cancer Prediction - FastAPI App

This project is a machine learning deployment using FastAPI for breast cancer prediction. It takes medical feature inputs from a web form and predicts whether the tumor is Malignant (Cancer) or Benign (Not Cancer).



📦 Clone This Repository

git clone https://github.com/Sumit-123singh/Breast-cancer-detection-system-using-Machine-Learning
cd Breast-cancer-detection-system-using-Machine-Learning

⚙️ Environment Setup

✅ Python 3.10 or above is recommended

Create a virtual environment:

python -m venv venv
source venv/bin/activate    # On Windows: venv\Scripts\activate

Install dependencies:

pip install -r requirements.txt

🚀 Run the App Locally

gunicorn app:app

Visit: http://127.0.0.1:8000

Swagger Docs: http://127.0.0.1:8000/docs

🧠 ML Model Details

Model Type: Logistic Regression Classifier

Dataset: breast cancer.csv (from UCI repository or scikit-learn)

🌐 Deployment (Render)

Build Command:

pip install -r requirements.txt

Start Command:

gunicorn app:app

Environment Variables (on Render dashboard):

SECRET_KEY=<your-secret-key-generated>
FLASK_ENV=production
MODEL_PATH=model.pkl

Generate secret key using:

python -c "import secrets; print(secrets.token_urlsafe(32))"

Note: Ensure gunicorn is included in requirements.txt



## 💧 Project Structure

```text
ml_fastapi_deploy/
├── app.py                          # FastAPI main application
├── model.pkl                       # Trained ML model (Logistic Regression)
├── requirements.txt                # Python dependencies
├── .gitignore                      # Git ignore rules
├── README.md                       # Project documentation

├── templates/                      # HTML templates
│   └── index.html                  # Web form for user input

├── static/                         # Static files (images, CSS)
│   └── images/
│       ├── alert_image.png
│       ├── img.jpg
│       └── okay_img.jpg

├── anaconda_projects/              # Model training and dataset
│   ├── breast_cancer_prediction_model.ipynb  # Jupyter Notebook for training
│   ├── breast cancer.csv                     # Dataset (UCI Breast Cancer)
│   └── project_filebrowser.db                # Anaconda project metadata
```



👨‍💻 Author
Sumit Singh
ML Enthusiast | Backend Developer
