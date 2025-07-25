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
https://github.com/Data-PrepeZ/Data_Prepez.git
cd Data-Prepez
pip install -r requirements.txt
```

---

## ⚡ Quick Start

```python
from dataprepez import AutoPreprocessor
import pandas as pd

# Load dataset
df = pd.read_csv("your_data.csv")

# Initialize the preprocessor
prep = AutoPreprocessor(target='target_column', type='tabular')

# Run preprocessing
X_clean, y = prep.fit_transform(df)
```

---

## 🧪 Example Notebooks

Check out the [examples/](examples/) folder:
- 🧹 `tabular_demo.ipynb` – Basic tabular preprocessing
- 📝 `nlp_cleaning.ipynb` – NLP cleaning pipeline *(coming soon)*
- 📈 `timeseries_demo.ipynb` – Time series preprocessing *(coming soon)*

---

## 🗂️ Project Structure

<details>
<summary>Click to expand</summary>

```
Data-Prepez/
├── dataprepez/
│   ├── tabular/
│   │   ├── __init__.py
│   ├── nlp/
│   │   ├── __init__.py
│   ├── timeseries/
│   │   ├── __init__.py
│   ├── core/
│   │   ├── __init__.py
│   │   └── preprocessor.py
│   └── __init__.py
├── tests/
│   └── test_preprocessor.py
├── examples/
│   └── tabular_demo.ipynb
├── README.md
├── setup.py
├── requirements.txt
└── LICENSE
```

</details>

---

## 🤝 Contributing

We welcome contributions from the community!  
To contribute:

1. Fork this repository  
2. Create your feature branch: `git checkout -b feature/YourFeature`  
3. Commit your changes: `git commit -m "Add your feature"`  
4. Push to the branch: `git push origin feature/YourFeature`  
5. Open a pull request 🎉

---

## 👥 Team

- **Bala Mosay J** – Team Lead, Core Developer  
- **Allwyn Jeffo Raj A** – NLP Module Developer  
- **Rasik S** – Time Series & Testing  

---

## 📄 License

This project is licensed under the [MIT License](LICENSE).

---

## 🌟 Show Your Support

If you like this project, please ⭐ star this repository and share it with others!

---

> _Clean your data, prep it like a pro — with **Data-Prepez**_
