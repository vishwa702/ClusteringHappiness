# Analysis of Global Happiness Indicators

This repository contains the code, analysis, and application developed for the project **"Analysis of Global Happiness Indicators"**. The project explores a less subjective alternative to analyzing global happiness, offering actionable insights and recommendations for policymakers.

---

## Abstract

The World Happiness Report is an annual study measuring global happiness. The report has been criticized for having subjectivity in its observations. In this project, we provide a less subjective analysis by clustering countries from the years 2015 to 2022 while ignoring the happiness score that contains inherent biases. In its place, we use principal component analysis to develop a bias-free custom happiness score. We also identify GDP and social support to be the most influential features for a country’s happiness using regression analysis. Moreover, we analyze countries for fluctuation in happiness on a yearly basis to find the most stable or unstable countries. Finally, we develop an application for government officials to extract key insights from our analysis.

---

## Methodology

To analyze global happiness data, we began by sourcing information from the World Happiness Report (2015–2022). Subjective features such as the Happiness Score and Dystopia Residual were omitted to reduce inherent biases. Clustering algorithms including K-means, OPTICS, DBSCAN, and K-medoids were applied to identify patterns in the data, with K-means clustering (K=3) emerging as the most interpretable and robust method based on validation indices like the Davies-Bouldin Index, Calinski-Harabasz Index, and Silhouette Coefficient. A custom happiness score was then developed using Principal Component Analysis (PCA), which projected data points onto a direction of maximum variance in the feature space, offering a bias-free metric for ranking countries. These clusters and scores enabled us to provide yearly recommendations for countries, targeting the most impactful features for improvement. Additionally, regression analysis highlighted GDP and Social Support as significant contributors to happiness, while identifying evolving trends in the importance of different variables.

---

## Demo

### Visualizations
![Recommendation for Ukraine](https://user-images.githubusercontent.com/54744950/235325657-a311287a-f1d9-4930-9392-1b9815b6cfd5.png)  
**Fig 1. Recommendation for Ukraine in 2022**  

![Progression of Canada](https://user-images.githubusercontent.com/54744950/235323133-f9ee86d3-1793-41c5-ba9b-4ec1b7a4eb46.png)  
**Fig 2. Progression of Canada (2015-2022)**  

![DBSCAN and K-Means](https://user-images.githubusercontent.com/54744950/235325682-a93ce3c2-0d12-469c-ad21-9b123821565b.png)  
**Fig 3. Cluster Analysis of DBSCAN & K-Means**  

![K-medoids & OPTICS](https://user-images.githubusercontent.com/54744950/235325690-fb2bb22d-6204-49ab-9508-b7132a77c1eb.png)  
**Fig 4. Cluster Analysis of K-medoids & OPTICS**  

![Year-wise Clusters](https://user-images.githubusercontent.com/54744950/235325698-a810221a-ac7a-426b-b1ad-ced648c4d604.png)  
**Fig 5. Year-wise Clusters found by K-Means**  

![Regression Analysis](https://user-images.githubusercontent.com/54744950/235325710-132282f0-f852-4cb9-ac51-c1b412ddcd98.png)  
**Fig 6. Regression analysis on the contribution of features on happiness score from 2015 to 2022**  

---

## Application Features

1. **Recommendations Dashboard**:
   - Generate policy suggestions for a given country.
2. **Trend Analysis**:
   - Track the happiness progression of any country over time.
3. **Cluster Visualizations**:
   - Explore clustering results for each year using multiple algorithms.

---

## Technologies Used

- **Programming Language**: Python
- **Libraries**:
  - Data Analysis: Pandas, NumPy, Scikit-learn
  - Visualization: Matplotlib, Seaborn
  - Application: Streamlit

---

## How to Run

1. Clone this repository:
   ```bash
   git clone https://github.com/username/analysis-global-happiness.git
   cd analysis-global-happiness
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Launch the application:
   ```bash
   streamlit run app.py
   ```

4. Access the app in your browser at `http://localhost:8501`.

---

## Acknowledgement

This project was developed in collaboration with [Ali Parsaee](https://github.com/yoguy12345) under the guidance of Prof. Joerg Sander at the University of Alberta. For a detailed overview, refer to the [Project Report](https://drive.google.com/file/d/1vok2c326OzMwTz9LuCAkXDwTuIQBzyL1/view?usp=sharing).

---
