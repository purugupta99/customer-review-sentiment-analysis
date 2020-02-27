### Customer Review Sentiment Analysis

#### Pipeline
- Data Preprocessing
	- A data corpus of 2 GB is given in the form of HTML WebPages
	- Using lxml formating and BeautifulSoup the relevant data like keywords, urls, reviews etc. have been extracted and can be found in processed.csv

- Text processing
	- change case to lower
	- tokenize text and remove puncutation
	- remove words that contain numbers
	- remove stop wordsremove empty tokens
	- lemmatize text
	- remove words with only one letter

- Feature extraction
	- Apply sentiment analysis on the text processed data to get score for positive, neutral, negative and compound features
	- Adding number of characters and words as a feature for all samples
	- Adding document feature and term frequency feature for all samples

- Classification
	- Clustering – apply k-means clustering to cluster positive and negative reviews based on the new features
	- Vader model – Use vader model to analyze the overall sentiment of the review to predict if it is positive or negative