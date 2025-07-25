# 🚀 Data-Prepez

**A fast, scalable, and intelligent data preprocessing library for machine learning workflows.**

Data-Prepez is an open-source Python library designed to simplify and accelerate the data preprocessing stage of machine learning. It automatically handles missing values, encoding, scaling, type detection, and supports tabular, text (NLP), and time series data — all while scaling efficiently to millions of rows.

---

## 📌 Features

- ✅ Automatic detection of numerical, categorical, and text features  
- ✅ Missing value imputation (mean, median, mode, forward fill, etc.)  
- ✅ One-hot and label encoding  
- ✅ Standard, MinMax, and Robust scaling  
- ✅ NLP preprocessing (cleaning, tokenization, lemmatization)  
- ✅ Time series resampling, smoothing, windowing  
- ✅ AutoPipeline: one-liner `fit_transform()` interface  
- ✅ Modular and production-ready design  
- ✅ Large dataset support (planned: Dask, Modin integration)  
- ✅ Compatible with Pandas, NumPy, and Scikit-learn  

---

## 🔧 Installation

> 📦 PyPI release coming soon!

For now, clone the repository:

```bash
git clone https://github.com/YOUR_USERNAME/Data-Prepez.git
cd Data-Prepez
pip install -r requirements.txt


## ⚡ Quick Start
python
Copy
Edit
from dataprepez import AutoPreprocessor
import pandas as pd

# Load dataset
df = pd.read_csv("your_data.csv")

# Initialize the preprocessor
prep = AutoPreprocessor(target='target_column', type='tabular')

# Run preprocessing
X_clean, y = prep.fit_transform(df)
🧪 Example Notebooks
Check out the examples/ folder:

🧹 tabular_demo.ipynb

📝 nlp_cleaning.ipynb

📈 timeseries_demo.ipynb (coming soon)

🗂️ Project Structure
arduino
Copy
Edit
Data-Prepez/
├── dataprepez/
│   ├── tabular/
│   ├── nlp/
│   ├── timeseries/
│   ├── core/
│   └── utils/
├── tests/
├── examples/
├── README.md
├── setup.py
├── requirements.txt
└── LICENSE
🤝 Contributing
We welcome contributions from the community!
To contribute:

Fork this repository

Create your feature branch: git checkout -b feature/YourFeature

Commit your changes: git commit -m "Add your feature"

Push to the branch: git push origin feature/YourFeature

Open a pull request 🎉

👥 Team
Bala Mosay J – Team Lead, Core Developer

Allwyn Jeffo Raj A. – NLP Module Developer

Jaiprasanth M. – Time Series & Testing

📄 License
This project is licensed under the MIT License.

🌟 Show Your Support
If you like this project, please ⭐ star this repository and share it with others!
