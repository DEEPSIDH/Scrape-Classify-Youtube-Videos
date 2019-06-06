# Scrape-Classify-Youtube-Videos
________________________________________________________________________________
Scrape &amp; Classify Youtube Videos in 6 categories based on their descriptions.  

Around 1500 videos were scraped for the following six categories:  
  
1.Travel blogs  
2.Science and Technology  
3.Food  
4.Manufacturing  
5.History  
6.Art and Music  
________________________________________________________________________________  

This project has three sections:  
  1.Scraping Youtube Videos  
  2.Preprocessing of Data   
  3.Developing Machine Learning Models for classification of said videos.  

The two sections are discussed further:  
# 1.Scraping Youtube Videos  
VideoID,Title and Description were extracted from various Youtube videos by sending queries
through the Google Youtube API V3 . This was facilitated through an unique key that is generated when
you enable the particular API in a project on console.developers.google.com

To avoid misuse of the particular API, Youtube will only return a maximum of 50 videos per query.
Collecting a minimum of 1700 videos per category at a rate of 50 videos per query was not feasible. This
was overcome by taking into account the last token that was received by the program and it was run again
till the token suggested that it was the last page.

# 2.Scraping Youtube Videos  
The data collected needed to be cleansed of Social Media Site names,hyperlinks,punctuation,contact
information and any other URLs also.
Lemmatization was also done so as to prepare the data better for further use.
Tokenization, stopwords, punctuation removal was also done.
CountVectorization and Tf-idf were also done.

# 3.Developing Machine Learning Models  
 A total of 3 models were developed for the classification.  
  1.Naive-Bayes Classifier  
  2.Random Forest Classifier   
  3.Convolutional Neural Network  

The described sections have their own notebooks.  
