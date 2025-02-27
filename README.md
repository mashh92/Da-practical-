Edt

Figmat

Fun

Gutions

Window

Help

Import nitk

inport

re

text="1111 Text Summariaztion 000 is an NLP technige that extracts text froma large amount of data. It is the process of identifying the most imporant Imeaningful information Sin a document and compressing it 7into a shorter version by preserving its meaning. Types: Extractive summarization and Abstractive summariza To perform extractive summarization, @we calculate the sentence weights and choose the first 'n' sentence w maximum weight, (The weights are calculated on the basis of the word frequencies ]***

A

Removing numbers inside square brackets text = re.sub(r'\/\*\/','', text)

#Fixing extra spaces

text = re.sub(r\s+','', text)

Removing special characters like [] {} *

text = re.sub(r'[\[\][*]','',text)

Removing non-alphabet characters formatted text = re.sub('[^a-zA-Z]','',text)

print(formatted_text)
