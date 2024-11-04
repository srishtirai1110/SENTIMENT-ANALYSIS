#import nltk
from textblob import TextBlob
#from newspaper import Article


#nltk.download('punkt')
with open('mytext.txt','r') as f:
    text = f.read()

#url = 'https://www.cnbc.com/2024/09/19/stock-market-today-live-updates.html'

#article = Article(url)
#article.download()
#article.parse()
#article.nlp()

#text = article.summary
#print(text)

blob = TextBlob(text)
sentiment = blob.sentiment.polarity # -1 to 1
print (sentiment)
