# Stacking_Sentiment_Analysis <br>
Twitter is a social media site, where people interact with the other users by posting messages called tweets, about topics they include in their posts using hashtags. Twitter is a rich source of data. Analyzing the tweets can give you important and interesting insights about what people are talking about, the sentiments of people, their opinions towards a particular topic/brand and the general trends in society. <br> <br>
Sentiment analysis refers to analyzing an opinion or feelings about something using data like text or images, regarding almost anything. Sentiment analysis helps companies in their decision-making process. For instance, if public sentiment towards a product is not so good, a company may try to modify the product or stop the production altogether in order to avoid any losses.<br> <br>

Text preprocessing steps include a few essential tasks to further clean the available text data. It includes tasks like:-
<br> <br>
1. Stop-Word Removal : In English words like a, an, the, as, in, on, etc. are considered as stop-words so according to our requirements we can remove them to reduce vocabulary size as these words don't have some specific meaning<br>

2. Lower Casing : Convert all words into the lower case because the upper or lower case may not make a difference for the problem. And we are reducing vocabulary size by doing so. <br>

3. Stemming : Stemming refers to the process of removing suffixes and reducing a word to some base form such that all different variants of that word can be represented by the same form (e.g., “walk” and “walking” are both reduced to “walk”). <br>

4. Tokenization : NLP software typically analyzes text by breaking it up into words (tokens) and sentences. <br>
## Algo's
### Base SVM model with TF-IDF
The intuition behind TF-IDF is as follows : <br>
If a word w appears many times in a sentence S1 but does not occur much in the rest of the Sentences Sn in the corpus, then the word w must be of great importance to the Sentence S1. The importance of w should increase in proportion to its frequency in S1 (how many times that word occurs in sentence S1), but at the same time, its importance should decrease in proportion to the word’s frequency in other Sentence Sn in the corpus. <br>
 **Mathematically, this is captured using two quantities: TF and IDF. The two are then multiplied to arrive at the TF-IDF score.** <br>
TF (term frequency) measures how often a term or word occurs in a given document.  <br>
IDF (inverse document frequency) measures the importance of the term across a corpus. In computing TF, all terms are given equal importance (weightage). However, it’s a well-known fact that stop words like is, are, am, etc., are not important, even though they occur frequently. To account for such cases, IDF weighs down the terms that are very common across a corpus and weighs up the rare terms. IDF of a term t is calculated as follows: <br>
