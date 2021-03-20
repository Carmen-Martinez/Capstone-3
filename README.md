## Rock Music Analysis

The purpose of this project is to find patterns in rock music, specifically identifying subgenres in rock. Music streaming companies, like Spotify and Apple Music, have a goal to keep their customers on their app for as long as possible. Because subgenres are hard to identify, it may be difficult to recommend a specific music preference to a customer which decreases session time on the app. My analysis hopes to find a solution to this issue. 


### Methods Used:
<ul>
<li>Data Cleaning</li>
<li>Descriptive and Inferential Statistics</li>
<li>Data Visualization (matplotlib/seaborn)</li>
<li>Model Prep</li>
<li>Dimensionality Reduction(FAMD)</li>
<li>Machine Learning Models(DBSCAN, Agglomerative)</li>
</ul>


### Technologies:
<ul>
<li>Python</li>
<li>Jupyter Notebook</li>
<li>Pandas</li>
<li>Matplotlib/Seaborn</li>
<li>Sklearn</li>
<li>and other relevant libraries</li>
</ul>

### Project Description:
The project was retrieved from kaggle: https://www.kaggle.com/lukaszamora/history-of-rock-19502020. I used pandas for data manipulation and data analysis along
with Matplotlib, Seaborn, Numpy, and Scikit-Learn (for the models). Originally the dataset only quantitative variables, but I decided to change some to categorical variables because it seemed appropriate considering the column descriptions in the kaggle page. Once I categorized some of the variables, I generated some plots (in the future I will use plotly). Finally I ran the models. I first used a dimensionality reduction technique called FAMD, which is great for mixed data. Then I ran DBSCAN and Agglomerative models. The DBSCAN model only produced one cluster (epsilon=0.2, min_pts=5). For the agglomerative model, I specified 3 clusters (silhouette score=0.41), this produced clusters that weren't overlapping too much. The best model seems to be the agglomerative model.
