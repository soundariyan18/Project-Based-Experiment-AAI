<H3>NAME: <h3>soundariyan MN</H3>
<H3>REGISTER NO:212222230146</H3>
<H3>DATE:29-04-2025</H3>
<H1 Align="center">Project Based Experiment<H1>
<H3>Objective:<H3>
To perform sentiment analysis on Facebook data and filter for messages, comments, or posts with negative feedback.

# Program:
```py
import nltk
from nltk.sentiment import SentimentIntensityAnalyzer
nltk.download('vader_lexicon')
sia = SentimentIntensityAnalyzer()
facebook_data = [
  "I love the new feature! It's amazing.",
  "The service was terrible. I'm very disappointed.",
  "Great job on the update!",
  "The product quality is poor. I won't be buying again.",
  
]
negative_feedback = []

for message in facebook_data:
  sentiment_score = sia.polarity_scores(message)['compound']
  if sentiment_score < 0:  # Negative sentiment
      negative_feedback.append(message)
print("Negative Feedback:")
for feedback in negative_feedback:
  print(feedback)
```
# Output:
![image](https://github.com/user-attachments/assets/801c5d08-cea8-49a3-9354-399a40d54dc3)

# Inference:
A sentiment analysis project using Facebook data provides valuable learning experiences in data handling, text processing, sentiment analysis, and ethical considerations, while also honing communication, problem-solving, and project management skills.
