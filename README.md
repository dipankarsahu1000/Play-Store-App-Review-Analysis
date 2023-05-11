<h1> Problem Statement</h1>

There are two datasets available. One containing the details of the apps like its name, category to which it belongs to, the rating it has, its size, etc. While the other one contains details regarding the reviews given to the apps by the users and the sentiments attached to the reviews.
To explore and analyze the data to discover key factors responsible for app engagement and success.


<h1> Business Context </h1>

The Play Store is a repository for a multitude of apps. The humongous data it holds can be prospectively very useful.

The developers need to know the standards to strive for and the factors to take care of in their apps. The users also rely on the app's ratings and reviews to make an informed decision.

However, with such a vast amount data it can become a difficult to understand what makes an app successful in the market. So that is why it is beneficial to perform an exploratory data analysis on the datasets. It can aid us in identifying the trends, patterns and the relationships between various features of the data. This will help the developers to understand and work on the key factors that help make their apps more successful and help them in making data-driven decisions when designing and marketing their apps.



<h1> Approach </h1>

The following are the steps that are going to be followed:

1. Getting to Know the Data: Loading the datasets, checking the information in the datasets and examining different characteristics of the datasets like the number of rows and columns, null/missing values and duplicate values.
2. Understanding the Variables: Diving deeper by checking each of the variables (columns) of the datasets, understanding what each of the variables stand for, studying some of the basic statistical details of the numerical variables and checking for the unique values for each of the columns.
3. Data Wrangling: Taking care of the duplicate values, tending to the null/missing values, transforming the datatypes of the columns whenever required, etc.
4. Data Visualization & Experimenting with Charts: Understanding the relationships between variables with the help of suitable charts and coming up with some useful insights.
5. Conclusion: Discussing the important insights that we have gained from the analysis.


<h1> Getting to Know the Data </h1>

1. Number of Rows and Columns:
    - The Play Store Dataset has 10841 rows and 13 columns.
    - The User Dataset has 64295 rows and 5 columns.

2. Number of Duplicate Values:
    - There are 483 duplicate values in the Play Store Dataset.
    - There are 33616 duplicate values in the User Reviews Dataset.

3. Missing/Null Values:
    - There are total 1487 missing/null values for the Play Store Dataset.
    - There are total 107457 missing/null values for the User Reviews Dataset.


<h1> Understanding The Variables </h1>

1. All the variables in the Play Store Dataset are:

    - App: The name of the app.
    - Category: The category to which the app belongs to.
    - Rating: The ratings (out of 5) given by the users to that particular app.
    - Reviews: The number of reviews given by the users to that particular app.
    - Size: The space required in the phone's memory to install that app.
    - Installs: The number of times that app has been installed by various users.
    - Type: Tells whether the app is free or paid.
    - Price: The price of the app if the app is paid, the price would be 0 if it is free.
    - Content Rating: The Age group for which the app is suitable for.
    - Genres: The genre(s) of the app.
    - Last Updated: The date on which the latest update for the app was released.
    - Current Ver: The current version of the app.
    - Android Ver: The android version that can support the app.

2. All the variables in the User Reviews Dataset are:

    - App: The name of the app.
    - Translated_Review: The reviews given by the users translated to English.
    - Sentiment: The sentiment of the users towards that app. It can be Positive, Negative or Neutral.
    - Sentiment_Polarity: A measure of the sentiment. It has a range of [-1, 1]. The more negative the number is, the more negative is the sentiment and       the more positive it is, the more postive is the sentiment. If it is somewhere around 0, then it is a neutral sentiment.
    - Sentiment_Subjectivity: It defines how subjective are the reviews, or simply, by how much are the sentiments influenced by the personal opinions of       the user. It has a range of [ 0, 1]. More closer it is to 0, the more objective (unbiased or free of personal opinions) are the sentiments, and the       more closer it is to 1, the more subjective (biased or influenced by personal opinions) are the sentiments.
    
    
<h1> Data Wrangling </h1>

On the Play Store dataset and User Reviews dataset, some of the following procedures were used:

- Taking care of the duplicate values: Duplicate values should be first examined and then after consideration, the duplicate values may be dropped/removed while keeping only one of the occurrences of the duplicate values. If the duplicate values are not important at all, then they may be removed completely.

- Taking care of the null values: If the null/missing values are not important to the analysis, then they can be simply removed. Otherwise, an appropriate value (like the mean, mode or median, depending on the case) can be imputed in place of the null values.

- Transforming the datatypes of the columns: Wherever the values under a column are not of a datatype fit for further analysis, then those values should be transformed such that the new values are more suitable for the analysis.

- Sanity Checks: These are a set of basic procedures performed on the datasets to quickly evaluate its correctness and quality. For example, checking if a set of values is within its expected range.

- Merging the User Reviews Dataset with the Play Store Dataset: If it helps in generating more insights, then the datasets can be merged appropriately.

<h1> Data Visualization & Experimenting with charts </h1>

1. Univariate Analysis: Univariate analysis involves examining the distribution of the variables in the dataset separately. Generally, the following charts are used for univariate analysis:
    - Bar Plot: It displays the frequency or count of each category in a categorical variable using bars of equal width and height. It is suitable for displaying the frequency or count of each category in a categorical variable.
    - Pie Chart: It displays the relative proportions of different categories in a categorical variable as slices of a pie.
    - Count Plot: It is similar to a bar plot. The main difference between a bar plot and a count plot is that a bar plot can be used for both numerical and categorical data, while a count plot can only be used for categorical data.
    - Histogram: It displays the distribution of a single continuous variable by dividing it into intervals (bins) and counting the number of observations in each bin.
    - Box Plot: It displays the distribution of a numerical variable by showing the quartiles, median, and outliers.
    - Line Plot: A chart that displays the trend or changes in a single variable over time or another continuous variable by connecting the data points with straight lines. Line plots can also be used to show the relationship between two numerical variables.
    - Word Cloud: It is a visual representation that displays the frequency or importance of different words in a text by their size. The more frequent or important a word is in the text, the larger or more prominent it appears in the word cloud.

2. Bivariate Analysis: Bivariate analysis involves examining the relationship between two variables in the dataset. Usually, the following charts are used for univariate analysis.  Usually, the following charts are used for univariate analysis:
    - Correlation Heatmap: It displays the correlation between multiple variables in a matrix format, where the values are represented by colors and/or numbers.
    - Scatter Plot: It displays the relationship between two continuous variables. Each point on the scatterplot represents a combination of values of the two variables.
    - Regression Plot: It displays the relationship between two numerical variables and estimates a regression line that best fits the data.



<h1> Conclusion </h1>

From this Exploratory Data Analysis, we have mainly gained the following insights:

- A vast number of people use apps belonging to the categories of 'Game', 'Tools' and 'Communication'. So the developers may try to target these categories.

- There are more number of free apps than the paid ones. So this goes on to say that the market is huge for the free apps.

- If the developers are interested in developing paid apps, then they should be created for the categories of 'Finance', 'Lifestyle' or 'Events'. As these are the categories which have the most number of paid apps, so it can be said that the users don't mind paying for the apps belonging to these categories.

- The developers should focus on apps with a content rating of 'Everyone', as more number of people use such apps.

- Although users generally don't prefer apps of larger sizes, but still if the developers have to develop a large-sized app (more than 80 MB), then they should create for the categories of 'Game' or 'Family', as most of the large-sized apps are concentrated in these categories.

- The apps should be updated regularly, because recently updated apps are generally well-received.

- Apps belonging to the 'Game' category should be developed more carefully as it tends to receive very high negative reviews if something goes wrong with the app. Also, the game apps also gets very high positive reviews if it is well-designed and satisfies the users. So, the game apps are a slippery slope.

- Most of the apps get positive ratings. So if the app is well-made and there is nothing wrong with it, then it is not that hard to get positive reception.


<h1> Challenges Faced </h1>

- The issue of multiple duplicate values was there. The duplicate values were dropped carefully making sure that no other values get affected.

- There were multiple null/missing values in our datasets. The null values were either dropped or replaced with an appropriate value, such that the overall data doesn't get affected.

- Transforming the values under certain columns into more suitable datatypes for an easier analysis (for example, string to integer). This part also consisted removed unwanted characters like '$', '+', etc, from the values being transformed.

- Choosing the right kind of charts for the visualisations and making sure that visualisation output is comprehensible.

<h1> Libraries Used </h1>

- numpy
- pandas
- matplotlib.pyplot
- seaborn
- missingno
- wordcloud
- datetime
- warnings
