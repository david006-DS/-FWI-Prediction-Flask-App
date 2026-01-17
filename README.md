
# 🔥 FWI Prediction Flask App

A machine learning web application that predicts the Fire Weather Index (FWI) using environmental parameters. Built with Flask and Ridge Regression model.

## 🌟 Overview

The Fire Weather Index (FWI) is a numeric rating of fire intensity. This application uses a trained Ridge Regression model to predict FWI based on various environmental factors such as temperature, humidity, wind speed, and other meteorological parameters.

## ✨ Features

- **Real-time Predictions**: Get instant FWI predictions based on input parameters
- **User-friendly Interface**: Clean and intuitive web interface
- **Machine Learning Powered**: Uses Ridge Regression with StandardScaler preprocessing
- **Responsive Design**: Works on desktop and mobile devices
- **Fast and Efficient**: Optimized model loading and prediction

## 🛠️ Technologies Used

- **Backend**: Flask (Python web framework)
- **Machine Learning**: scikit-learn (Ridge Regression, StandardScaler)
- **Frontend**: HTML5, CSS3
- **Data Processing**: NumPy, Pandas
- **Model Serialization**: Pickle

## 📦 Installation

### Prerequisites
- Python 3.8 or higher
- pip (Python package manager)

### Steps

1. **Clone the repository**
```bash
git clone https://github.com/david006-DS/-FWI-Prediction-Flask-App.git
cd -FWI-Prediction-Flask-App
```

2. **Create a virtual environment**
```bash
python -m venv .venv
```

3. **Activate the virtual environment**

On Windows:
```bash
.venv\Scripts\activate
```

On macOS/Linux:
```bash
source .venv/bin/activate
```

4. **Install dependencies**
```bash
pip install -r requirements.txt
```

5. **Run the application**
```bash
python application.py
```

6. **Open your browser**
Navigate to `http://127.0.0.1:5000/`

## 🚀 Usage

1. Navigate to the homepage
2. Click on "Start Predicting" button
3. Enter the following parameters:
   - **Temperature** (°C)
   - **Relative Humidity** (%)
   - **Wind Speed** (km/h)
   - **Rain** (mm)
   - **FFMC** (Fine Fuel Moisture Code)
   - **DMC** (Duff Moisture Code)
   - **ISI** (Initial Spread Index)
   - **Classes** (Fire classification)
   - **Region** (Geographic region code)
4. Click "Predict FWI"
5. View your prediction result

### Sample Input Values

**Moderate Fire Risk:**
- Temperature: 25
- RH: 60
- Ws: 15
- Rain: 0
- FFMC: 85
- DMC: 25
- ISI: 8
- Classes: 1
- Region: 2

## 🧠 Model Information

### Ridge Regression Model
- **Algorithm**: Ridge Regression (L2 regularization)
- **Preprocessing**: StandardScaler for feature normalization
- **Training**: Model trained on historical fire weather data
- **Serialization**: Models saved using Pickle format

### Model Files
- `models/rid.pkl`: Trained Ridge Regression model
- `models/sc.pkl`: Fitted StandardScaler for data preprocessing

## 📁 Project Structure

```
-FWI-Prediction-Flask-App/
│
├── .venv/                      # Virtual environment
├── models/                     # Trained models
│   ├── rid.pkl                # Ridge Regression model
│   └── sc.pkl                 # StandardScaler model
├── templates/                  # HTML templates
│   ├── index.html             # Homepage
│   └── home.html              # Prediction form page
├── notebook/                   # Jupyter notebooks (training)
├── application.py              # Main Flask application
├── requirements.txt            # Python dependencies
├── README.md                   # Project documentation
└── .gitignore                 # Git ignore file
```

## 📸 Screenshots

### Homepage
![Homepage](screenshots/homepage.png)

### Prediction Form
![Prediction Form](screenshots/prediction-form.png)

### Results
![Results](screenshots/results.png)

## 🤝 Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository
2. Create a new branch (`git checkout -b feature/YourFeature`)
3. Commit your changes (`git commit -m 'Add some feature'`)
4. Push to the branch (`git push origin feature/YourFeature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## 👨‍💻 Author

**David Quaye-Fio**
- GitHub: [@david006-DS](https://github.com/david006-DS)
- Email: dquayefio813@gmail.com

## 🙏 Acknowledgments

- Fire weather data sources
- scikit-learn documentation
- Flask framework documentation
- Open source community

## 📞 Support

If you have any questions or need help, please open an issue in the GitHub repository.

---

Made with ❤️ by David Quaye-Fio
