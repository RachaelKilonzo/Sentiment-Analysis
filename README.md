# Sentimeent Analysis on Death Note
![ryuk gif](https://user-images.githubusercontent.com/93233240/145114947-acae8dd9-9e4b-4454-91e1-aeac3cabc7ae.gif)

## Intoduction
Despite not being an avid fan of anime in comparison to Webtoons or Manhuas or even Manhwas, I thought Death Note would be quite interesting to do a sentiment analysis on. Perhaps this choice was guided by the lessons that I learnt from the manga as a child. Lessons on the fact that people are not infallible, it is easy to get lost in the pursuit of one’s goals and the fact that there is no absolute right or wrong. This is my very first work on this topic and , so feel free to correct me on anything weird or improvement ideas.

The choice for this project is based on:
- **Inspiration:** This is heavily inspired by Xaviers work analysing the sentiments on [Star Wars](https://www.kaggle.com/xvivancos/analyzing-star-wars-movie-scripts) data set
- **Data Source:** I went through the tedious process of scraping the transcripts from [Anime de English](https://anime-de-english.com/category/transcripts/) and making them slightly intelligible. Some Webscrapping was also done to get transcripts from [Death Note's fandom](https://deathnote.fandom.com/wiki/Death_Note_(anime)/List_of_Episodes/)
- **Author and illustrator:**  Tsugumi Ohba and Takeshi Obata whose sheer imagination and artistic skill created one of the most iconic manga and anime series. 
![8Vg1s0v](https://user-images.githubusercontent.com/93233240/138996937-4fc952d7-972f-44a4-b38e-613f0f8639e7.jpg)

## Libraries
Libraries used were: RWeka, memery, ggimage, magick, tidyverse, tm, wordcloud, wordcloud2, tidytext, reshape2, knitr, gridExtra, magick, memery, ggimage, igraph, ggraph, syuzhet, textdata, stringr, readxl, tidyr.

## Word Cloud of the most frequent words.
![4](https://user-images.githubusercontent.com/93233240/145253323-18d33381-3111-4479-a6af-8464b2ca2b59.png)

A bit of data cleaning was done to remove duplicates and align the capitalization of characters
## Text Mining
A bunch of functions are applied to remove punctuation, extra white space, make all characters lower case, remove numbers and remove common English words called stopwords. 
This predefined function is going to clean the text from:

## Charty Characters.
![1](https://user-images.githubusercontent.com/93233240/145224154-ce20ad9c-7706-451c-b868-849eca5eafe7.png)
- **Light and L** as expected have the largest percentage of dialogue in the anime. They are the main characters. An antagonist and protagonist
- **Misa, Soichiro, Matsuda and Ryuk** come in as the second most talkative group.
- **Aizawa, Near, Higuchi and Rem** rounding up the 10 most talkative characters.

## Opinion Mining
### BING Lexicon 
The Bing Lexicon categorizes the words into a binary fashion of either positives and negatives.
![2](https://user-images.githubusercontent.com/93233240/145231207-79e241cc-cd46-4118-8440-4777e14dbd78.png)
Variations of the root word kill (killed, kill and killing), death (die, death, dies) and wrong are predominant as the most popular negative words while right, like, well and good are the most popular positive words. This is correlation to the archetypes of the storyline. The questions on right and wrong actions in relation to human life. Death and murder as commited by Light.
### NRC Lexicon
The nrc lexicon groups the words in 10 moods:positive, negative, anger, anticipation, disgust, fear, joy, sadness, surprise, trust.
![3](https://user-images.githubusercontent.com/93233240/145233053-869ff087-b357-4d09-9672-f00fba14f661.png)
The positive and negative are the most prevalent moods. Additionally, there is also a lot of fear trust and anticipation in the anime.

## AFINN Lexicon
Afinn Lexicon ranks every word from -5 to 5, where:
- -5 being the most negative
- +5 being the most positive

![6](https://user-images.githubusercontent.com/93233240/145258731-2911018b-d859-4dfc-ba6c-4c0e09eda293.png)
This is the word count distribution over the intensity of sentiments
## Bigram Networks
For the purpose of visualizing a connection between the words. The most interesting connection is that Kira is linked to the hubs Light, catch, Kill and real.
Obvious combinations are: FBI and Agent, Cell and Phone, death and note, Light and Yagami. Sakura and TV e.t.c.

![5](https://user-images.githubusercontent.com/93233240/145255851-cd9c1d72-6de8-4d47-9f68-6febecc1da32.png)

More diagrams and code can be viewed above and suggestions are welcomed.
