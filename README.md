# Text-Analysis
Extract data from websites and perform NLP operation and save result in excel file

# Input
Input file (excel) consist of website links

# Web Scrapping
Using Newspaper and Article library: Extract only and only main article and title of webpage.

# Operations:
**Positive Score**: This score is calculated by assigning the value of +1 for each word if found in the Positive Dictionary and then adding up all the values.

**Negative Score**: This score is calculated by assigning the value of -1 for each word if found in the Negative Dictionary and then adding up all the values. We multiply the score with -1 so that the score is a positive number.

**Polarity Score**: This is the score that determines if a given text is positive or negative in nature. It is calculated by using the formula: 
Polarity Score = (Positive Score – Negative Score)/ ((Positive Score + Negative Score) + 0.000001)
Range is from -1 to +1

**Subjectivity Score**: This is the score that determines if a given text is objective or subjective. It is calculated by using the formula: 
Subjectivity Score = (Positive Score + Negative Score)/ ((Total Words after cleaning) + 0.000001)
Range is from 0 to +1

**Average Sentence Length** = the number of words / the number of sentences

**Percentage of Complex words** = the number of complex words / the number of words 

**Fog Index** = 0.4 * (Average Sentence Length + Percentage of Complex words)

**Average Number of Words Per Sentence** = the total number of words / the total number of sentences

**Complex Word Count**
Complex words are words in the text that contain more than two syllables.

**Word Count**: We count the total cleaned words present in the text by 
  > removing the stop words 
  > removing any punctuations like ? ! , . from the word before counting.

**Syllable Count Per Word**: exceptions like words ending with "es","ed" by not counting them as a syllable.

**Personal Pronouns**: counts of the words - “I,” “we,” “my,” “ours,” and “us”. Special care is taken so that the country name US is not included in the list.

**Average Word Length**:
Sum of the total number of characters in each word/Total number of words

# Conditions
Use only those positive and negetive and stopwords which are given, not from NLTK Library
