# SpaceX Stage 1 Landing Prediction – Data Science Capstone  

## 📌 Overview  
This project builds a **machine learning pipeline** to predict whether a SpaceX Falcon 9 rocket's **Stage 1** will successfully land, using data from the **public SpaceX API** and **Wikipedia**. The aim is to help a fictional company **SpaceY** compete with SpaceX by forecasting landings, potentially saving **~$100 million USD per launch**.  

We collected, processed, visualized, and modeled real launch data to achieve an **83% accuracy rate** across multiple models.  

---

## 🚀 Why This Project is Useful  
- **Cost Savings** – Successful Stage 1 landings allow rocket reusability, drastically reducing launch costs.  
- **Data-Driven Decisions** – Predictive insights help determine whether a launch should proceed.  
- **Interactive Visualization** – Dashboards and maps for deeper launch analysis.  
- **Educational Value** – Demonstrates the end-to-end data science process, from collection to deployment.  

---

## 📊 Methodology  

1. **Data Collection**  
   - Pulled structured data from the **SpaceX public API**.  
   - Scraped additional launch details from **Wikipedia**.  
   - Merged and cleaned datasets for modeling.  

2. **Data Wrangling**  
   - Created binary classification label:  
     - `1` = Successful landing  
     - `0` = Failure  
   - One-hot encoded categorical variables.  
   - Standardized numerical features.  

3. **Exploratory Data Analysis (EDA)**  
   - **Visualization**: Analyzed payload mass, orbit, site success rates.  
   - **SQL Analysis**: Queried DB2 database for launch patterns.  
   - **Folium Maps**: Mapped launches, landings, and key site proximities.  

4. **Interactive Dashboard**  
   - **Pie Chart**: Success rates by site.  
   - **Scatter Plot**: Payload mass vs. success rate, colored by booster type.  

5. **Modeling**  
   - Algorithms: Logistic Regression, SVM, Decision Tree, KNN.  
   - Hyperparameter tuning with **GridSearchCV (cv=10)**.  
   - Achieved ~**83.33% accuracy** across models.  

---

## 📈 Results  
- All models showed **similar accuracy (~83%)**.  
- Models tended to **over-predict successful landings**.  
- Best-performing launch sites: **KSC LC-39A** and **CCAFS SLC-40**.  
- Interactive visualizations revealed **orbit-type correlations** and payload mass trends.  

---

## 🔮 Future Improvements  
- Collect **more historical and recent data** for model stability.  
- Experiment with **ensemble learning** (Random Forest, XGBoost).  
- Integrate **weather conditions** as a predictive feature.  
- Deploy as a **real-time prediction service**.  

---

