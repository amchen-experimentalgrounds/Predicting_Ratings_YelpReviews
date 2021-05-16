# Predicting Ratings of Yelp Reviews
This was an assignment done in Semester 1, 2020 for the subject COMP30027 Machine Learning.  I was a 3rd-year undergrduate student at the time.

The task was to classify Yelp reviews into 1, 3 or 5-star reviews. 
The given data included the text of Yelp reviews, review metadata (reviewer_id, business_id, review_id, date, vote_funny, vote_cool, vote_useful) and some preconstructed features using Doc2Vec.
The official assigment objectives were to build 3 classifiers and write a report.

My personal objectives were to:
1. become more familiar with textual data.
2. explore whether my (linguistics-inspired) features would achieve a good model performance.
3. get experience with a wider variety of models, but without using neural networks or anything too resource-intensive / ambitious.

This model was ranked #7 (in "preliminary results", I guess) and #15 (final result) out of 264.

# My approach
It is common to include n-grams (sequences of n words) as a feature. I used 1-grams and 2-grams. 2-grams are essential to capturing the meaning of the text. Here is an illustrative example: "the food was **not good**." Other than that, I deviated from the norms of natural language processing by considering capitalisation and punctuation. Ideally, I should have done some further processing, but instead, I merely took the decision to not remove them. Nonetheless, this seemed to improve the performance of the models. Apart from that, it was mostly a problem of selecting a suitable model with the right parameters to achieve the best performance in testing.

I was probably the only student to intentionally leave in punctuation (other students unintentionally left it in?). I believe other top-scoring models opted to use more advanced models, such as neural networks. Next time I do NLP tasks, I should consider that too.

My final paper is included in this repository. It's not ground-breaking, but feel free to have a read if you want to see my thought process. The code is also included, but it's not particularly well-commented. It was mostly to show the markers that my work was original. Nonetheless, it should be more than readable.
