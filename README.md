# Concrete Compressive Strength Prediction

This project predicts the **compressive strength of concrete** using a **hybrid machine learning and deep learning approach**. It combines **Random Forest**, **XGBoost**, and a **custom PyTorch Neural Network**, and applies **ensemble averaging** to improve predictive performance.

---

## 🌟 Features

- Predict concrete compressive strength based on mix ingredients and curing age.
- Uses **feature engineering**: binder ratios, water/cement ratio, total binder, aggregate ratio.
- Compares multiple models:
  - Random Forest
  - XGBoost
  - PyTorch Neural Network
  - Ensemble Averaging
- Early stopping, Batch Normalization, and LeakyReLU used in neural network for improved performance.
- R² performance of ensemble: **0.91**, outperforming individual models.

---

## 📊 Dataset

The dataset used is the **Concrete Compressive Strength Dataset** from **Kaggle**:

- [Concrete Compressive Strength Dataset](https://www.kaggle.com/datasets/elikplim/concrete-compressive-strength-data-set)

It contains 1030 samples with 8 features:

- Cement (kg/m³)  
- Blast Furnace Slag (kg/m³)  
- Fly Ash (kg/m³)  
- Water (kg/m³)  
- Superplasticizer (kg/m³)  
- Coarse Aggregate (kg/m³)  
- Fine Aggregate (kg/m³)  
- Age (days)  

Target: **Concrete compressive strength (MPa)**

---

## 📊 Model Performance

| Model          | R² Score |
|----------------|----------|
| Ensemble Avg   | 0.910    |
| XGBoost        | 0.907    |
| Stacking       | 0.904    |
| Random Forest  | 0.891    |
| PyTorch NN     | 0.884    |

---

## 🛠️ Technologies

- Python 
- PyTorch
- scikit-learn
- XGBoost
- Pandas & Numpy (data processing)
- Matplotlib (visualizations)

---

## ⚡ Project Structure

```

concrete_strength_project/
│
├─ notebook/             # Jupyter notebook for EDA and model development
└─ README.md

````

---

## 📈 Example Input

| Feature          | Example Value |
| ---------------- | ------------- |
| Cement (kg/m³)   | 540           |
| Slag (kg/m³)     | 0             |
| Fly Ash (kg/m³)  | 0             |
| Water (kg/m³)    | 162           |
| Superplasticizer | 2.5           |
| Coarse Aggregate | 1040          |
| Fine Aggregate   | 676           |
| Age (days)       | 28            |

**Predicted Compressive Strength (EnsembleAvg)**: 82.45 MPa

---

## 📊 Visualizations

* R² comparison bar chart
* Actual vs Predicted scatter plots
* Ensemble contribution plot

These plots demonstrate **how the ensemble improves predictions** over individual models.

---

## 💡 Future Work

* Deploy with **Docker** for easy cloud deployment.
* Add **confidence intervals** for predictions.
* Integrate **historical data visualization** for user input comparison.
* Experiment with **stacking ensemble methods** for further improvement.

---

## 📄 License

This project is **open-source** and available under the [MIT License](LICENSE).

---

## 👩‍💻 Author

**Amira Qadry** – [GitHub](https://github.com/yourusername) | [LinkedIn](https://www.linkedin.com/in/amiraqadry/)
