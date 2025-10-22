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
├─ data/                  # Dataset CSVs
├─ models/                # Saved model files (.pt, .pkl)
├─ notebooks/             # Jupyter notebooks for EDA and model development
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
