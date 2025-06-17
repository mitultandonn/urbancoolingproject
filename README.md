# Urban Cooling Risk Prediction using IoT, AI, and Human Behavior

## Project Overview

This project presents a data-driven, human-centric approach to assessing Urban Heat Risk (UHR) in Penrith, Western Sydney — a region highly affected by the Urban Heat Island (UHI) effect. By integrating IoT sensor data, machine learning models, and human behavioral indicators like clothing and activity levels, the project predicts urban heat risk at a granular level.

Unlike conventional UHI studies, this project combines environmental and human factors into a single unified framework — useful for urban planners, councils, and public health authorities aiming for real-time, adaptive interventions.

## Tools and Technologies

- Languages: Python
- Libraries: Pandas, Scikit-learn, Seaborn, Matplotlib
- ML Models: Random Forest, Logistic Regression, SVM, KNN, Decision Tree
- Environment: Jupyter Notebook / Google Colab
- Data Sources:
  - Australian Bureau of Meteorology
  - OpenAQ
  - Local council population and infrastructure datasets

## Features

- Developed a Discomfort Index combining environmental (Temp, RH, PM2.5) and behavioral (Clothing Factor, Activity Level) variables
- Built classification models to predict Urban Heat Risk levels (Low, Medium, High)
- Identified Random Forest as the best performer with 94% accuracy
- Created visualizations for feature importance, discomfort indices, risk class distribution, and model predictions

## Methodology

### Data Preprocessing
- Cleaned and merged multiple datasets (sensor + population + built environment)
- Engineered behavioral features: Clothing Factor, Activity Level

### Discomfort Index Models
Three discomfort indices (DI1, DI2, DI3) were designed using weighted sums:
DI1 = 0.3T + 0.2RH + 0.1PM2.5 + ... - 0.1CF + 0.1AL
DI2 = ...
DI3 = ...

### Model Training
Used multiple classifiers to predict UHR class (Low, Medium, High):
- Logistic Regression
- Random Forest
- KNN
- SVM
- Decision Tree

Random Forest achieved the best performance:  
Accuracy: 94%, Weighted F1 Score: 0.94

## Visual Outputs

- Confusion matrix showing performance across risk levels
- Feature importance plot (PM2.5 most influential)
- Pairplot of Discomfort Indices vs Risk Classes
- Urban heat risk distribution across areas
- Heat risk probability vs Temperature

## Key Learnings

- Real-time urban cooling solutions benefit greatly from integrating human behavioral proxies
- IoT, AI, and human-centric design create more accurate and adaptable urban risk models
- Environmental temperature alone is not the best indicator of heat stress

## Folder Structure
urban-cooling/
├── data/ # Source datasets (sensor, weather, population)
├── notebooks/ # Jupyter notebooks for analysis and modeling
├── models/ # Trained model files (.pkl)
├── images/ # Output visualizations
├── report.pdf # Academic paper / conference submission
├── README.md # This file



## Future Work

- Add temporal dynamics using time-series heat data
- Incorporate satellite imagery or geospatial overlays
- Use Explainable AI (XAI) for stakeholder transparency
- Validate models across different cities (e.g., Chandigarh, Mumbai)

## License

This project is open-sourced under the MIT License.

## Authors

- Mitul Tandon | Deakin University  
- Kevin Lee  
- Kanaka Sai Jagarlamudi

Feel free to reach out or fork the repo to extend the project for your own city.



