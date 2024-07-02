# Youtube-Text-Data-Analysis

The revolution of social media sites has also attracted the users towards video sharing sites, such as YouTube. The online users express their opinions or sentiments on the videos that they watch on such sites.

According to the latest YouTube statistics, the video-sharing platform has 2.6 billion users worldwide as of 2022 (Statista, 2022). It’s ranked as the second-most popular social network, and the only platform that has more active users than YouTube is Facebook. 

The objective is to automatically recognize and categorize opinions expressed in the comments to determine overall sentiment of the user.

Sentiment analysis helps data analysts within large enterprises gauge public opinion, conduct nuanced market research, monitor brand and product reputation, and understand customer experiences. 

## Business Problem Statements

Observations on the following are made:
1. Sentiment analysis on YouTube comments.
2. Exploratory data analysis on positive sentences
3. Exploratory data analysis on negative sentences.

## Dataset

- The dataset includes data gathered from the (up to) 200 listed videos on YouTube that are contained within the trending category each day in the US.
- The headers in the comments file are:
   - **video_id**
   - **comment_text**
   - **likes**
   - **replies**
 
## Data Analysis Using Python

1. Polarity determination using TextBlob
2. WordCloud representation of sentiments
3. Removal of StopWords
4. Emoji’s Analysis

### Polarity determination using TextBlob
- Use **TextBlob's sentiment feature** to determine polarity for each comment.
- ***Polarity values range from -1 to +1***.

<p align="center"><img width="854" alt="image" src="https://user-images.githubusercontent.com/71536311/193256220-ddf59988-c6b3-4ea4-890a-7691f19d32e6.png"></p>

### WordCloud representation of sentiments
- Perform **WordCloud** of positive and negative sentences.
- To generate a word cloud, convert all comments into string format using the **join function**.
- Polarity ***1 indicates a positive sentence***, polarity ***-1 indicates a negative sentence***.

<p align="center"><img width="692" alt="image" src="https://user-images.githubusercontent.com/71536311/193200845-7235ef53-2351-415d-8588-80e60768c976.png"></p>

### Removal of STOPWORDS
- As you can see from the below image, the highlighted words don't add any value to the sentiments.

<p align="center"><img width="685" alt="image" src="https://user-images.githubusercontent.com/71536311/193201401-2fdc9b93-916f-4f01-8717-99bca1327a6c.png"></p>

- Remove stop words using **WordCloud's Stopword feature**, which already has all the stop words present, to get the precise WordCloud, otherwise inaccurate data will be provided.

#### Positive WordCloud
<p align="center"><img width="454" alt="image" src="https://user-images.githubusercontent.com/71536311/193393814-f1a81a38-31c7-4119-b06b-06c227205c0e.png"></p>

#### Negative WordCloud
<p align="center"><img width="461" alt="image" src="https://user-images.githubusercontent.com/71536311/193393794-abea3e36-a5f9-4590-8dd1-e3c8f82378cc.png"></p>

### Emoji’s Analysis
- Extract emojis from comments for analysis.
- The frequency of each emoji can be calculated using the **counter feature** in **Collections libraries**.
- **Counter's most_common function** will return the top 10 emojis that are frequently used.
- Separate emojis and frequency in order to plot a graph using **plotly**.

<p align="center"><img width="503" alt="image" src="https://user-images.githubusercontent.com/71536311/193393744-97ca1eed-2849-49ee-8154-3eb9bd21e2f2.png"></p>

## Tools Used
![Jupyter Notebook](https://img.shields.io/badge/jupyter-%23FA0F00.svg?style=for-the-badge&logo=jupyter&logoColor=white)   ![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)   ![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)   ![Matplotlib](https://img.shields.io/badge/Matplotlib-%23#ffffff.svg?style=for-the-badge&logo=Matplotlib&logoColor=white)   ![Plotly](https://img.shields.io/badge/Plotly-%233F4F75.svg?style=for-the-badge&logo=plotly&logoColor=white)   ![NumPy](https://img.shields.io/badge/numpy-%23013243.svg?style=for-the-badge&logo=numpy&logoColor=white)

- **Jupyter Notebook** is used as IDE.
- Among the **Python libraries**, **Pandas** and **NumPy** are used for handling data, preprocessing, and mathematical operations, respectively.
- **Plotly, Seaborn**, and **Matplotlib** are used for visualizing plots.

For more details, please go through the Jupyter Notebook attached above.
