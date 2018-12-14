# Recommend-System-Baseline
Some common recommendation system baseline, with description and link.

1. Pop : POP (popular products): this model recommends the most popular products in the training set. Though POP is simple, it is often a strong baseline in certain domains.

2. ItemKNN : this model is based on the co-occurrences of products in the baskets. This is one of the most common item-to-item recommendation in the form users who bought X also bought Y.

3. prod2vec : a word2vec version for learning the product representations by corresponding a basket as a sentence and a product in the basket as a word. A basket’s representation is calculated as the mean of the products contained in the basket. Given a basket, we compute the cosine similarities between its representation and all potential products, and pick top N-similar products.

4. doc2vec : a model for learning text representations. We apply doc2vec to obtain the product
representations from their titles. A basket’s representation is calculated as the mean of the products contained in it. Given a basket, we calculate the cosine similarities between the basket’s representation and all potential products, and pick top-N similar products.

5. BPR-MF:  It optimizes the matrix factorization in a pairwise manner with Bayesian Personalized Ranking loss, which aims to maximize the difference between positive
and negative items. It does not model the sequential signals.

6.  FMC: is is a simplied version of factorized personalized Markov Chain (FPMC) which does not include user personalized behaviours.

7. FPMC : is approach combines matrix factorization machine with Markov Chain for next item recommendations. The proposed approach captures both user-item preferences and user sequential behaviours.

8. HRM : It is a Hierarchical Representation Model which captures both sequential and general user tastes by introducing both linear and nonlinear pooling operation for historical transaction aggregation. Here, the average aggregation is adopted.

9. PRME : This is model was originally proposed for POI recommendation. It utilizes metric embedding to learn user and item embeddings as well as the user check-in sequences.

10. TransRec : This model applies the idea of translating embeddings to sequential recommendation. It views users as relation vectors and assumes that the next item is determined by user’s recent interacted item plus the user relation vectors.
11. Caser : It models user past historical interactions with both hierarchical and vertical convolutional neural networks. It also considers the skip behaviors and the whole
network is optimized by minimizing the cross entropy. 

12. AttRec : This model combines self-attention and metric learning at the same time, is a sequence-based reommendation system algorithm.

13. BASTEXT : a model of texts and shopping basket data, uses the texts for addressing the cold-start problem and uses the basket data for improving the performance of text representations. 

### Reference:
The the above is taken from paper below,
1. Learning Representations from Product Titles for Modeling Large-scale Transaction Logs, https://arxiv.org/abs/1811.01166 
2. Next Item Recommendation with Self-Attention, https://arxiv.org/pdf/1808.06414
