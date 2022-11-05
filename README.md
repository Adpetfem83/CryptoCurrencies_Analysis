
#  Cryptocurrencies

### An analysis using unsupervised Machine Learning algorithm to discover unknown patterns.

## Resources
* Dataset from [CryptoCompare](https://min-api.cryptocompare.com/data/all/coinlist)
* Software: Python 3.7.9, Anaconda 4.9.2 and Jupyter Notebooks 6.1.4
* Libraries: `Scikit-learn`, `Plotly`, `hvPlot`, `Pandas`

![bannerimage](https://github.com/Adpetfem83/Cryptocurrencies_Analysis/blob/main/Images/Human_Image.png)

## Overview

In this project the purpose of this analysis was to use data provided to provide a report and visualization of currently traded cryptocurrencies which  can be grouped together in order to create a new classification system. This report would then be used by **Accountability Accounting** to offer a new investment portfolio in the exciting world of cryptocurrency to its teeming customers. 

We are using the data that has no known outcome, then, we needed to preprocess it to fit unsupervised `Machine Learning` model which will help us to run a clustering algorithm that will enable us to group the cryptocurrencies.

For this challenge we applied:

* **Data Preprocessing** (Selection, Transformation, Scaling) - refers to the process of helping to prepare data for `Machine Learning` Algorithms.
* **Elbow Curve** - this is a method to determine the best number of clusters needed for the algorithm to group the objects by.
* **Principal Component Analysis (`PCA`)** - is a statistical technique to speed up machine learning algorithms when the number of features is too high.
* **Clustering Algorithms (`KMeans`)** - is the process of grouping similar objects/data points into clusters.
* **Visualization (`hvPlot`, `Plotly`)** - these are graphic libraries that allows us to create 2D and 3D graphs such as, scatter plots for visualization.

# Data Frame before Cleaning
![DataFrame_before_cleaning](https://github.com/Adpetfem83/Cryptocurrencies_Analysis/blob/main/Images/DataFrame%20before%20Cleaning.png)
 
# Data Frame after cleaning
![DataFrame_after_cleaning](https://github.com/Adpetfem83/Cryptocurrencies_Analysis/blob/main/Images/DataFrame%20after%20Cleaning.png)

# Data Frame with three PCA
![DataFrame_3_PCA](https://github.com/Adpetfem83/Cryptocurrencies_Analysis/blob/main/Images/DataFrame_with_3_PCA.png)

# Data Frame for plotting hvplot Scatter

![DataFrame_for_plotting_hvplot_Scatter](https://github.com/Adpetfem83/Cryptocurrencies_Analysis/blob/main/Images/DataFrame_for_Plotting_hvplotScatter.png)



###  Results

The original dataset used contained 1,252 entries, however, only 1,144 cryptocurrencies were traded. The data was further manipulated to remove `null values` and to produce cryptocurrencies that had a total number of mined coins greater than 0. Eventually, the results identified 532 tradable cryptocurrencies. 

![cryptotable](https://github.com/Adpetfem83/Cryptocurrencies_Analysis/blob/main/Images/Tradable%20Currencies.png)

The **Elbow Curve** method showed the slope at 4. This is the number of clusters that was used for the `KMeans` algorithm.

![Elbow](https://github.com/Adpetfem83/Cryptocurrencies_Analysis/blob/main/Images/Elbow_Curve.png)

The clusters are plotted in a 3D scatter plot for visualization.

![3DScatter](https://github.com/Adpetfem83/Cryptocurrencies_Analysis/blob/main/Images/3D_Scatter_with_PCA.png)

![hvplot Scatter](https://github.com/Adpetfem83/Cryptocurrencies_Analysis/blob/main/Images/hvplot.scatter.png)


