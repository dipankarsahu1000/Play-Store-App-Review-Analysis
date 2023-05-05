<h1> Problem Statement and Business Context </h1>

<b> The Play Store apps data has enormous potential to drive app-making businesses to success. Actionable insights can be drawn for developers to work on and capture the Android market.
Each app (row) has values for category, rating, size, and more. Another dataset contains customer reviews of the android apps.
To explore and analyze the data to discover key factors responsible for app engagement and success. </b>

The Play Store is a repository for a multitude of apps. The humongous data it holds can be prospectively very useful.

The developers need to know the standards to strive for and the factors to take care of in their apps. The users also rely on the app's ratings and reviews to make an informed decision.

However, with such a vast amount data data it can become a difficult to understand what makes an app successful in the market. So that is why it is beneficial to perform an exploratory data analysis on the datasets. It can aid us in identifying the trends, patterns and the relationships between various features of the data. This will help the developers to understand and work on the key factors that help make their apps more successful and help them in making data-driven decisions when designing and marketing their apps.

There are two datasets available. One containing the details of the apps like its name, category to which it belongs to, the rating it has, its size, etc. While the other one contains details regarding the reviews given to the apps by the users and the sentiments attached to the reviews.

<h1> Approach </h1>

The following are the steps that are going to be followed:

1. Getting to Know the Data: Loading the datasets, checking the information in the datasets and examining different characteristics of the datasets like the number of rows and columns, null/missing values and duplicate values.
2. Understanding the Variables: Diving deeper by checking each of the variables (columns) of the datasets, understanding what each of the variables stand for, studying some of the basic statistical details of the numerical variables and checking for the unique values for each of the columns.
3. Data Wrangling: Taking care of the duplicate values, tending to the null/missing values, transforming the datatypes of the columns whenever required, etc.
4. Data Vizualization & Experimenting with Charts: Understanding the relationships between variables with the help of suitable charts and coming up with some useful insights.
5. Conclusion: Discussing the important insights that we have gained from the analysis.
6. Challenges Faced: Mentioning the challenges faced during the analysis and how they were dealth with.

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
- Taking care of the duplicate values.
- Taking care of the null values.
- Transforming the datatypes of the columns
- Sanity Checks
- Merging the User Reviews Dataset with the Play Store Dataset

<h1> Data Vizualization & Experimenting with charts </h1>

Following types of chart were used:
 
- Correlation Heatmap
- Bar Plot
- Pie Chart
- Count Plot
- Histogram
- Box Plot
- Regression Plot
- Line Plot
- Word Cloud

<h1> Conclusion </h1>

From this Exploratory Data Analysis, we have mainly gained the following insights:

- A vast number of people use apps belonging to the categories of Game, 'Tools' and 'Communication'. So the developers may try to target these categories.

- There are more number of free apps than the paid ones. So this goes on to say that the market is huge for the free apps.

- If the developers are interested in developing paid apps, then they should be created for the categories of 'Finance', 'Lifestyle' or 'Events'. As these are the categories which have the most number of paid apps, so it can be said that the users don't paying for the apps belonging to these categories.

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
