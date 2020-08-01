# COVID-19 Tweet Analysis using NER

<ul>
<li> This project uses Named Entity Recognition (NER) for analysis of tweets from Twitter. At a time, 1000 realtime tweets are extracted from Twitter based on given keyword.
<li> NER is performed for determining top 10 locations which might be affected the most due to Covid-19 pandemic.
<li> Reference of the code is taken from <i>Source: https://algorithmia.com/blog/text-mining-tweets-named-entity-recognition</i>
<li> For more details of the project, refer <i>Project Report.pdf</i> file.
<li> For getting a gist of the project, refer <i>NLP_Tweet_Analysis_Demo.mp4</i> file.
</ul>

## Prerequisites
<ol>
<li> Install "tweepy" module with command:

        pip install tweepy

<li> Install "Algorithmia" module with command:

        pip install algorithmia

<li> Install "openpyxl" module with command:

        pip install openpyxl

</ol>

## How to run the project
<ol>
<li> Clone the project and open TweetAnalysis.py file.
<li> There are two files: "InputTweet.xlsx" which contains 1000 sample input tweets and "Output.txt" which contains sample output.
<li> You need to first create an account in Algorithmia. You can go at <i>https://algorithmia.com/signup</i> and create an account.
<li> After creating account, you will get an API key in your dashboard. Copy and paste that API key in line number 9 in TweetAnalysis file.
<li> You also need to create a Twitter Developer account. After creating Twitter Developer account, you will get 4 keys: API key, API Secret key, Access token, Access token secret.
<li> Copy these 4 keys on line numbers 19, 20, 21 and 22 respectively in TweetAnalysis.py file.
<li> In line 42, add the path where you want to save your InputTweets.xlsx file.
<li> Save the changes and run TweetAnalysis.py file
<li> In terminal you will find top 10 locations with their tweet counts. In InputTweets.xlsx, all 1000 extracted tweets will be saves and in Output.txt top 10 locations with their tweet counts will be saved.
</ol>

## Note
The program extracts 1000 tweets from Twitter. Sometime it may happen that it is not printing any output.
That is because it is not getting any LOCATION in those 1000 extracted tweets. It might have got NAME
or ORGANIZATION in those tweets. In such cases, run the program again for getting results.