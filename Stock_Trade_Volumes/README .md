
# Project Title

“A study of correlation between name, prices (high and low)  and trade volumes of stocks for years 2013-2018.”--- (Clustering-Unsupervised Learning, Regression-Supervised Learning.)


## Acknowledgements

 - DATA SOURCE: 
    Kaggle “S&P 500 stock data”
 - LINK : 

    Kaggle:

    https://www.kaggle.com/camnugent/sandp500


    Google Drive link for data file:

    https://drive.google.com/file/d/1r9mU2pb_fTA4VCGHGZP5mn3zrnqNsK29/view?usp=sharing

    Filename  :  all_stocks_5yr.csv

    Since the file size is greater than 25 MB, it could not be uploaded to GitHub. It can be downloaded from the Google drive link provided above. 
## Tech Stack 
   DATA EXPLORATION:
   
   pandas, matplotlib, matplotlib.pyplot,  matplotlib inline, numpy, seaborn in Python
   
   MACHINE LEARNING TECHNIQUES:

   sklearn library in Python
   KMeans from sklearn.cluster 
   LinearRegression from sklearn.linear_model 

 




## Documentation

This dataset contains historical stock prices(last 5 years from the date of upload, 2018) for all companies currently found on the S&P 500 index.

The aim is to draw a conclusion about/ find a correlation beteween volume of stocks traded  and factors such as stock name, price(high/low) and opening price of the stock. It is to check if we can predict high/low volume of stocks traded based off these factors, based on this study using both CLUSTERING  and REGRESSION techniques. 

The project aims to find hidden patterns in the unlabeled data, to capture paradigms that lead to high/low trade volume of stocks of all companies currently found on the S&P 500 index for the years(2013 – 2018). 


DATA EXPLORATION:

The dataset has 619040 entries and 7 columns, out of which I shall be using 619029 entries(after removing rows with NaN values.The data has stocks' transaction date,opening price, closing price, high price, low price,volume, and Name. The volume(volume of stocks traded) is important to the stock market and the investors, because it shows how often the stocks of a certain type are traded the most. We want to see if there is a stock attribute that's associated with a higher trade volume.Pairplots were drawn between the columns using seaborn library.

After looking at the pairplot of all columns, I have selected to study the correlation between high & volume, low & volume, Name & volume. After dropping 3 columns (date, open, close) that clearly do not have as much correlation with volume, we will use Clustering to find out if those stocks with highest trade volumes have any common attributes like price(open, high, low,close) or name.

The dataset is very large, and it should be sufficient to draw conclusion about the factors affecting trade volumes of stocks.

MACHINE LEARNING TECHNIQUES:

The project aims at finding hidden patterns in the unlabeled data, which comprises of stocks of all companies currently found on the S&P 500 index for the years(2013 – 2018). Using the Clustering technique, (K-Means Clustering)which is Unsupervised learning, I have tried to learn about data by observing hidden correlations between data points. 

I have done further exploration by using Supervised Learning, (Linear Regression) to find if we can predict stock prices and hence counsel our clients.  Trade volume of stocks is the labeled data and names of stocks, high price, low price and opening price of the stock are the attributes of the stocks, used to study the factors affecting trade volumes of stocks. 




## Lessons Learned

It can be seen from all of the above findings from our studies using scatterplots and K-Means clustering, that there is no definite relationship or dependency,between price attributes(high, low, close or open) or name attributes and trade volume of the stocks. Although with every run of the program, a different set of clusters are formed, but a general trend that emerges everytime is that the price and the name atributes showed no, or very little correlation with high trade volume. This was further confirmed by our studies in linear regression, where the regression lines were almost parallel to the x-axis in each case, showing absolutely no correlation, between the variables and the volume. Therefore, it can be said with emphasis that stocks traded in high volume do not share any price attributes(high, low, close or open) or name attributes,as there is no correlation between the given attributes.

--There could be several reasons for our findings. Firstly, our dataset was not a Gaussian distribution as we have seen from our histograms above. The data is already skewed as seen earlier, in spite of it being a very large dataset.Therefore, inadequate sampling does not seem to be a likely factor here, considering the fact that a very large number of stock names(505 in all) were involved. However, we can make a better estimate if we check the percentage of stocks studied by us, compared to those that are traded in the stock market.Secondly, it is only to be expected that a stock with 'high' price value in a certain range will have its 'low' price value in a similar range, and any effect it will have on trade volume due to sudden fluctuations would be ironed out over a period of 5 years, which is our scope of study.(Implying that our dataset being large, and gathered over a long time weeds out any possibility of correlation with trade volume).

--From our thorough and exhaustive study of the dataset for the stocks traded in 5 years as above, with the given information in the dataset, we cannot provide any advice regarding the common attributes of highly traded stocks,except for maybe that BAC stocks are traded the most. At our end, we can further fine tune our study by :

1. Normalizing the data
2. Changing the number of clusters, although we have tried to do our best by using the optimal k-value from Elbow-plot.
3. Changing the 'init' value of the algorithm from default to a different value.
4. Changing the number of iterations of K-Means Clustering algorithm by changing the max_iter value.
5. It remains to be explored if adding data attributes, or, variables to make it a more inclusive study can lead us to some conclusion.
6. Splitting the large dataset into 2 or more parts , based on stock prices could be a major strategy to overcome this problem, given that the prices of higher-priced stocks are expected to run within a certain range of values, as compared to lower-priced stocks, which might run their valus run within a different range. Hence, segregation of stocks by splitting the dataset could be a major game-changer in drawing some conclusion about the factors affecting volume of a particular  stock traded, or what might affect low or high trade volumes of a particular stock in a given day.



# Hi, I'm Shweta! 👋

I am a Math teacher turned Machine Learning enthusiast, who loves to explore datasets. I like to disover interesting facts about and from the given  data. It is great fun to love to discover hidden patterns in the data and draw conclusions from it, using Mathematical methods.

