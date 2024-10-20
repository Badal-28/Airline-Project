# Airline (Sentimental Analysis)

## Tools Used - Python,NLTK,Pandas,Matplotlib,Seaborn

## Table of Contents
1. [Project Objective](#project-objective)
2. [Dataset Description](#dataset-description)
3. [Project Workflow](#project-workflow)
5. [Addressing The Issue](#addressing-the-issue)
6. [Possible Solutions and Strategy](#possible-solutions-and-strategy)

## Project Objective
The primary goal of this project is to identify optimal solutions to the challenges faced by travelers and develop strategies to enhance the services provided by various airlines. By conducting sentiment analysis on traveler feedback, we aim to extract valuable insights from the dataset to understand customer sentiments and experiences.

Through this analysis, we will evaluate the sentiment data contained within the provided dataframe, uncovering patterns and trends that can inform actionable recommendations. Ultimately, our objective is to improve the overall travel experience by addressing the concerns and preferences of passengers, thereby contributing to the strategic development of airline facilities and services.

## Dataset Description
Number of rows=1300+,Number of columns=19,The dataset includes detail about  aircraft , traveller_type , seat_type , route , date_flown , recommended 3 , trip_verified , rating , seat_comfort , cabin_staff_service , food_beverages , ground_service , value_for_money , entertainment

## Project Workflow
### 1.Here first we will know about sentimental analysis

#### What is Sentimental Analysis
Sentiment analysis is the process of analyzing digital text to determine if the emotional tone of the message is positive, negative, or neutral. Today, companies have large volumes of text data like emails, customer support chat transcripts, social media comments, and reviews. Sentiment analysis tools can scan this text to automatically determine the author’s attitude towards a topic. Companies use the insights from sentiment analysis to improve customer service and increase brand reputation. 

#### How does it work?
Sentiment analysis is an application of natural language processing (NLP) technologies that train computer software to understand text in ways similar to humans. The analysis typically goes through several stages before providing the final result.

##### Preprocessing
During the preprocessing stage, sentiment analysis identifies key words to highlight the core message of the text. Tokenization breaks a sentence into several elements or tokens.Lemmatization converts words into their root form. For example, the root form of am is be.Stop-word removal filters out words that don't add meaningful value to the sentence. For example, with, for, at, and of are stop words. 

#### What are the challenges in Sentimental Analysis
There are many challenges in Sentimental Analysis such as:
1.Tone , 2.Sarcasm, 3.Idioms , 4.Polarity, 5.Emojis, 6.Negations etc

### 2.Now we will talk about keyword Analysis
NLP technologies further analyze the extracted keywords and give them a sentiment score. A sentiment score is a measurement scale that indicates the emotional element in the sentiment analysis system. It provides a relative perception of the emotion expressed in text for analytical purposes. For example, researchers use 10 to represent satisfaction and 0 for disappointment when analyzing customer reviews.

### 3.Now we will talk about models that are used in Sentimental analysis

#### VADER VS roBERTA
One of the well-known rule-based algorithms is VADER from the NLTK package. According to developers, it is specifically attuned to sentiments expressed in social media. It is quite easy to implement yet a very powerful model. Another algorithm, I will talk about is a deep learning-based algorithm — Twitter-roBERTa from the TRANSFORMERS package. This model was pretrained with 124 million tweets and finetuned for sentiment analysis. Both of the models do not require any training, which means they can be directly applied to textual data out of the box.

##### VADER implementation
  For vader,clean your data as much as possible.As I said it will be quite easy to implememt
##### roBERTA implementation
  Twitter-roBERTa implementation is a bit more complicated than VADER, particularly 	because it does not provide a compound score we need to calculate ourselves.

#### Time Required for Predictions
In the above two sections, we saw that accuracy of roBERTa is much higher and reflects more reality. But in the world of data science, accuracy is not alone as a determining factor. Since computational resources are limited, one of the requirements for a model is that it should be computationally light as much as possible, particularly for production.It was already obvious from the implementation code snippets that VADER is much easier to apply compared to roBERTa. Moreover, in the following figure, you can see how much VADER is fast than roBERTa. On my personal laptop, VADER predicted sentiment of 1000 tweets only in 0.31 seconds. Contrary, roBERTa did the same task in 42.6 seconds (~130-fold slower).

Depending on the task and computational resources available one can select VADER or roBERTa. However, with a minimalistic amount of data pre-processing and incredible accuracy, Twitter-roBERTa seems more promising, especially if the amount of data is not so big.

### Note;Refer to the `AIRLINE PROJECT(1).pptx` for the more clear information along with visuals representing the issue.

## Addressing The Issue
We see that A320 is the busiest aircraft and Boeing 777 has least recommendation ratio in spite of being one of busiest aircraft. So, improving services of these aircrafts will give us more benefit.
Improvement in main areas(factors) of concern:
1.Cabin Staff Services
2.Vlaue For Money
3.Seat Comfort
4.Food and  Bevrages

## Possible Solutions and Strategy

### Cabin Staff Services 
1.Better training programs to ensure necessary skills required for delivering better services to travellers such as encouraging them to be approachable and attentive towards needs of passengers.
2.Conducting surveys:
     Conduct random surveys after the flight to know more about what are the specific concerns of passengers regarding the staff.
3.Incentives:
     Implement incentive programs or performance-based rewards to motivate staff and foster a culture of excellence. 

### Value For Money
1.Clear and transparent billing structure detailed breakdowns of fares and extra charges
2.Enhancing the quality of services 
3.Conduct surveys after flight mainly focusing on this factor
4.Give seasonal discounts and implement loyalty program offers for the passengers to the passengers who travelled more than once.
5.Monitor market trends and charge accordingly

### Seat Comfort
1.Improvement in seat material
2.Adjustable features such as headrests, armrests and footrests to passengers for more comfortability.
3.Maintenance of quality on a regular basis.
4.Maintain cleanliness of seats and bacteria free environment in the  aircraft.
5.Conduct surveys mainly focusing on feedback on hygiene .

### Food and Bevrages
1.Offering diverse meal options
2.High quality ingredients
3.Feedback from passengers regarding quality and quantity of food. 











