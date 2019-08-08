# Description
This project is connected with the Wrangling section of the Data Analyst nanodegree program offered by Udacity. The dataset used for wrangling (analyzing and visualizing) is the tweet archive of Twitter user @dog_rates, also known as WeRateDogs. WeRateDogs is a Twitter account that rates people's dogs with a humorous comment about the dog. These ratings almost always have a denominator of 10. The numerators, though? Almost always greater than 10. 11/10, 12/10, 13/10, etc. Why? Because "they're good dogs Brent." WeRateDogs has 4 million followers and has received international media coverage.

Real-world data rarely comes clean. Using Python and its libraries, the goal is to gather data from a variety of sources and in a variety of formats, assess its quality and tidiness, then clean it. This is called data wrangling. All the wrangling efforts are documented in this Jupyter Notebook, plus showcase them through analyses and visualizations using Python (and its libraries).

## Data Wrangling

> >Data wrangling consist in three main tasks:
>1. Gathering data
>2. Assessing data
>3. Cleaning data

### - Gathering Data for this Project

The data consist on three different pieces as described below and are integrated in a Jupyter Notebook titled `wrangle_act.ipynb`:

**The WeRateDogs Twitter archive**. csv file manually downloaded from a link containing: twitter_archive_enhanced.csv

**The tweet image predictions**, i.e., what breed of dog (or other object, animal, etc.) is present in each tweet according to a neural network. This file (`image_predictions.tsv`) is hosted on Udacity's servers and should be downloaded programmatically using the Requests library and the following URL: https://d17h27t6h515a5.cloudfront.net/topher/2017/August/599fd2ad_image-predictions/image-predictions.tsv

Each tweet's retweet count and favorite ("like") count at minimum, and any additional data you find interesting. Using the tweet IDs in the **WeRateDogs Twitter archive**, query the **Twitter API** for each tweet's **JSON data** using Python's **Tweepy** library and store each tweet's entire set of JSON data in a file called `tweet_json.txt` file. Each tweet's JSON data should be written to its own line. Then read this .txt file line by line into a pandas DataFrame with (at minimum) tweet ID, retweet count, and favorite count.

### - Assessing Data for this Project
After gathering each of the above pieces of data, assess them **visually and programmatically** for **quality** and **tidiness** issues. Detect and document at least **eight (8) quality issues and two (2) tidiness issues** in your `wrangle_act.ipynb` Jupyter Notebook.

### - Cleaning Data for this Project
Clean each of the issues you documented while assessing. Perform this cleaning in `wrangle_act.ipynb` as well. The result should be a high quality and tidy master pandas DataFrame (or DataFrames, if appropriate).

### Python Libraries
<br> For the analysis, the following python libraries are used:
<ul>
<li><b>sqlite3</b> for interacting with a local relational database.</li>
<li><b>pandas</b> and <b>numpy</b> for data ingestion and manipulation.</li>
<li><b>matplotlib</b> and <b>seaborn</b> for data visualization.</li>
<li><b>requests</b> for data gathering using urls.</li>
<li><b>tweepy</b> API used for gathering twitter data.</li>
<li><b>jupyter notebook</b>, for code development and analysis description.</li>
<li><b>json</b>, <b>os</b>, <b>time</b> and <b>pickle</b> for complete the used libraries.</li>
</ul>
# Data_Wrangling_TwitterAPI
