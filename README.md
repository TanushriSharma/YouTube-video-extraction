# YouTube-video-extraction

Many news channels today publish videos everyday covering the important events of the
day. Videos are an interesting mode of presenting information that might otherwise
seem dull in a text article and make it highly engaging for news readers and viewers.
The aim of this project is to create a system that extracts videos related to a news article
from YouTube.The videos might be uploaded by a news publisher or a user just sharing a video about
the event. This is a bilingual system, supporting both English and Hindi.

Key challenges
1. How to get videos around the article published time and rank them in terms of
relevancy.
2. How to fit it in Indian Language case, the common case is that the article will be in
Indian language while the video might be in English.

Approach to a solution

1. Since the articles from the dataset did not include the date or time of publishing,
there was no way of retrieving only those videos which were published around the
same time. So, this algorithm extracts the most recent videos relevant to the
content of the article.
2. In order to extract videos for articles whose text might be in a different language,
like Hindi, I used transliteration to generate the English counterpart of the
search query, and extracted videos based on those terms.
