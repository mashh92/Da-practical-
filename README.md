import re

import matplotlib.pyplot as plt

from nltk.corpus import stopwords

from nltk.probability import FreqDist

from nltk.tokenize import word tokenize from wordcloud import WordCloud

A

?

#Text paragraph to process

paragraph text = """

Hello all, Welcome to Python Programming Academy. Python Programming Academy is a nice platform to learn skills. It is difficult to get enrolled in this Academy.

tokenized_words = word_tokenize (paragraph_text)

stop_words_data = set(stopwords.words("english")) print("List of Stopwords: \n", stop words data)

filtered words_list = []

for word in tokenized words:

1f word.lower() not in stop words data and word.isalpha(): filtered words list.append(word)

print("\n Tokenized Words: \n", tokenized words)

print("\n Filtered Words: \n", filtered words list)
#Calculate word frequency distribution

freq_dist FreqDist(filtered words list)

#Path to the TrueType font on Ubuntu (use DejaVuSans-Bold or other available fonts)

font_path = "/usr/share/fonts/truetype/dejavu/DejaVuSans-Bold.ttf"

#Generate and display word cloud using the specified font

wordcloud = WordCloud (width=800, height=400, background_color='white', font_path=font_path).generate('.joi

#Display the word cloud

plt.figure(figsize=(10,5

)) plt.imshow(wordcloud, interpolation='bilinear')

plt.axis('off')

plt.title('Word Cloud of the Text')

plt.show()
