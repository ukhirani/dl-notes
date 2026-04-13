![[2sj4jrx3.png]]
# What is Recommendation Systems ?

- Recommendation systems are AI-driven tools that analyze user preferences, behaviors, and data to provide personalized suggestions.
- These systems leverage algorithms to predict user interests, helping them discover new items while boosting engagement and satisfaction for businesses.
- Widely used in e-commerce, streaming services, social media, and more, they enhance user experience by recommending relevant products, movies, music, or content
# Understanding Recommendation Systems 

- A recommendation system is a subclass of Information filtering Systems that seeks to predict the rating or the preference a user might give to an item.
- In simple words, **it is an algorithm that suggests relevant items to users**.

# Explicit Feedback vs. Implicit Feedback

- In [Recommender Systems](https://towardsdatascience.com/tag/recommender-systems/ "Recommender Systems"), machine learning models are used to predict the **rating _rᵤᵢ_ of a user _u_ on an item _i**._ At inference time, we recommend to each user _u_ the items _l_ having highest predicted rating _rᵤ**ᵢ**_.
- We therefore need to collect user feedback, so that we can have a ground truth for training and evaluating our models. An important distinction has to be made here between **explicit feedback** and **implicit feedback**.

![[pbs0eeg2.png]]

### Explicit Feedback

- **[Explicit feedback](https://en.wikipedia.org/wiki/Rating_scale#Rating_scales_used_online)** is a rating explicitly given by the user to express their satisfaction with an item.
- ***Examples are***: number of stars on a scale from 1 to 5 given after buying a product, thumb up/down given after watching a video, etc.
- This feedback provides **detailed information** on how much a user liked an item, but it is **hard to collect** as most users typically don’t write reviews or give explicit ratings for each item they purchase.

### Implicit Feedback

- **[Implicit feedback](https://en.wikipedia.org/wiki/Implicit_data_collection)**, on the other hand, assume that user-item interactions are an indication of preferences.
- ***Examples are***: purchases/browsing history of a user, list of songs played by a user, etc.
- This feedback is **extremely abundant**, but at the same time it is **less detailed** and **more noisy** (e.g. someone may buy a product as a present for someone else)
- However, this noise becomes negligible when compared to the sheer size of available data of this kind, and **most modern Recommender Systems tend to rely on implicit feedback**.
# Rating Matrix

![[nt3k48qv.png]]

- Once we have collected explicit or implicit feedbacks, we can create the **user-item rating matrix _rᵤᵢ_**.
- For **explicit feedback**, each entry in _rᵤᵢ_ is a numerical value—e.g. _rᵤᵢ =_ "stars given by _u_ to movie _i_"—or "?" if user _u_ did not rate item _i_.
- For **implicit feedback**, the values in _rᵤᵢ_ are a boolean values representing presence or lack of interaction—e.g. _rᵤᵢ =_ "did user _u_ watch movie _i_?".
- Notice that the matrix _rᵤᵢ_ is very sparse, as users interact with few items among all available contents, and they review even fewer items!
# Types of Recommendation System

Recommender system can be classified according to the kind of information used to predict user preferences as **Content-Based** or **Collaborative Filtering.**

![[ecufv8er.png]]

***Content Based*** ➡️ ([[AI and LLM/Content Based Filtering]])
***Collaborative Based*** ➡️ ([[AI and LLM/Collaborative Based Filtering]])

# Matrix Factorization for Recommendation

[[AI and LLM/Matrix Factorization for Recommendation]]
