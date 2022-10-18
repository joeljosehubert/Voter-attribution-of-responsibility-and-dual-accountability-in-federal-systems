# About the Project
This was submitted as part of my dissertation requirement for my masters in Data Science. The project uses natural language processing (NLP) to determine whether the voters can correctly attribute blame or responsibility on the governments. The project uses tweets to create the dataset.

## Datasets used
### Scraped tweets
The tweets were scraped and 6 datasets were made for each of the different policy areas in Kerala and Scotland. The dataset was then cleaned to focus on the content of the tweetsd and the twitter handles. The six datasets were the following 
1. Health in Kerala - this dataset is used to analyse the successful attribution of blame or responsibility by the tweets on matters of health in Kerala.
2. Health in Scotland - this dataset is used to analyse the successful attribution of blame or responsibility by the tweets on matters of health in Scotland.
3. Electricty in Kerala - This dataset is used to analyse the successful attribution of blame or responsibility by the tweets on matters of electricity in  in Kerala. The term electricity was used because an initialy analysis of tweets had revelaed that electricity is the umbrella term used for matters of energy in India.
4. Energy Crisis in Scotland - This dataset is used to analyse the successful attribution of blame or responsibility by the tweets on matters of electricity or energy in Scotland and draws a cpmparisdion with the tweets on erlectricity in Kerala. The term energy and crisis were together used as filters for scraping bevcause the initial analysis revealed the salience of this topic in the discourse with a looming winter.
5. GST in Kerala - GST is Goods and Services Tax and is a form of indirect tax applied on products. This dataset is used to analyse the successful attribution of blame or responsibility by the tweets on matters of GST in Kerala.
6. VAT in Scotland- VAT is Value added Tax and is a form of indirect tax applied on goods and services in Scotland. This dataset is used to analyse the successful attribution of blame or responsibility by the tweets on matters of VAT in Scotland.

## Model and approach explained
The tweets in the collected datasets were first analysed and were retained. After cleaning all the datasets and dropping irrelevant columns, we are loeft with 22 columns. NLTK is imported as th package for natural language processing and the tweets are tokenised and stemmed. A new column is created to establish the sentiment of each tweet as positive, negative or neutral; the sentimentvader package is used for this. 

The comibination of this new sentiment column is run along with terms that are used to refer to a particular government to analyse the attribution of responsibility. The column 'perception' captures if the response from the tweet is correct or nwrong attribution regardless of the positive or negative sentimentality.


