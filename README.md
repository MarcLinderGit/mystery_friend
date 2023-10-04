# Unmasking My Mystery Friend

In this project I will identify the mysterious sender of an an anonymous postcard using natural language processing and machine learning techniques as well as past writings from three potential senders: Emma Goldman, Matthew Henson, and TingFang Wu.
This intriguing journey begins with text exploration and feature extraction. I'll use a Bag-of-Words approach and a Naive Bayes classifier to unravel the secret friend's identity. Let's dive into the process step by step:

**1. Import Libraries**: I start by importing essential libraries, including scikit-learn's MultinomialNB for the classifier and CountVectorizer for text vectorization.

**2. Define bow_vectorizer**: I create a CountVectorizer object, which will help me convert text documents into numerical feature vectors.

**3. Vectorize Text**: All the writings from my friends are combined into a single document, and I use bow_vectorizer to transform them into feature vectors stored as friends_vectors.

**4. Prepare the Mystery Message**: A mysterious postcard arrives with a message. I vectorize this message into mystery_vector using the same vectorizer.

**5. Examine Friend's Writings**: I take a peek at samples from each friend's writings to familiarize myself with their writing styles.

**6. Build a Classifier**: I implement a Naive Bayes classifier (MultinomialNB) and store it as friends_classifier.

**7. Train the Classifier**: The classifier is trained on the feature vectors (friends_vectors) and corresponding labels (friends_labels).

**8. Make Predictions**: I use the trained classifier to predict the sender of the mysterious postcard based on the vectorized message (mystery_vector).

**9. Reveal the Mystery**: The moment of truth arrives! I reveal the sender by uncommenting the final print statement, unveiling the identity of my long-lost friend.

**10. Test with New Text**: For the ultimate test, I can input new text and see how the classifier performs. This flexibility allows me to use recent emails or texts to identify my friends.