# Abstract

The World Happiness Report is an annual study measuring global happiness. The report has been criticized for having subjectivity in its observations. In
this project, we provide a less subjective analysis by clustering countries from the years 2015 to 2022 while ignoring the happiness score that contains inherent
biases. In its place, we use principal component analysis to develop a bias-free custom happiness score. We also identify GDP and social support to be the most
influential features for a country’s happiness using regression analysis. Moreover, we analyze countries for fluctuation in happiness on a yearly basis to find the most
stable or unstable countries. Finally, we develop an application for government officials to extract key insights from our analysis.

# Methodology 

For identifying clusters of data, we experiment with K-means, OPTICS, DBSCAN, and K-medoids clustering algorithms. We find that K-means with K=3 gives the best and most interpretable clustering according to 3 cluster validation indices: Davies-Bouldin index, Calinski-Harabasz index, and silhouette coefficient. To develop a bias-free custom happiness score, we perform principal component analysis (PCA). This returns a direction in the feature space that covers maximum variation. We find the custom happiness score by projecting each data point to this direction. With the new score function, we rank the generated clusters to provide recommendations a given country for each year. While providing recommendations, we choose a feature that brings the most impact for the country to reach the next-best cluster. We also perform regression analysis on the data to find the importance of each considered variable that influence a country's happiness. 


# Demo

![image](https://user-images.githubusercontent.com/54744950/235325657-a311287a-f1d9-4930-9392-1b9815b6cfd5.png)

Fig 1.  Recommendation for Ukraine in 2022


![image](https://user-images.githubusercontent.com/54744950/235323133-f9ee86d3-1793-41c5-ba9b-4ec1b7a4eb46.png)\
Fig 2. Progression of Canada (2015-2022)


![image](https://user-images.githubusercontent.com/54744950/235325682-a93ce3c2-0d12-469c-ad21-9b123821565b.png)
 Fig 3. Cluster Analysis of DBSCAN & K-Means
 
 
![image](https://user-images.githubusercontent.com/54744950/235325690-fb2bb22d-6204-49ab-9508-b7132a77c1eb.png)
Fig 4. Cluster Analysis of K-medoids & OPTICS


![image](https://user-images.githubusercontent.com/54744950/235325698-a810221a-ac7a-426b-b1ad-ced648c4d604.png)
Fig 5. Year-wise Clusters found by K-Means


![image](https://user-images.githubusercontent.com/54744950/235325710-132282f0-f852-4cb9-ac51-c1b412ddcd98.png)
Fig 6. Regression analysis on the contribution of features on happiness score from 2015 to 2022.


# Acknowledement
This project was developed in collaboration with [Ali Parsaee](https://github.com/yoguy12345) under the guidance of Prof. Joerg Sander at the University of Alberta. 
Please refer to the complete [Project Report](https://drive.google.com/file/d/1vok2c326OzMwTz9LuCAkXDwTuIQBzyL1/view?usp=sharing) for more details. 
