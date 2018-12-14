# Recommend-System-Baseline

1. Pop : POP (popular products): this model recommends the most popular products in the training set. Though POP is simple, it is often a strong baseline in certain domains. [[python]](https://github.com/chenghu17/Sequential_Recommendation)

2. ItemKNN : this model is based on the co-occurrences of products in the baskets. This is one of the most common item-to-item recommendation in the form users who bought X also bought Y. [[pdf]](https://dl.acm.org/citation.cfm?id=372071), [[python]](https://github.com/caserec/CaseRecommender)

3. prod2vec : a word2vec version for learning the product representations by corresponding a basket as a sentence and a product in the basket as a word. A basket’s representation is calculated as the mean of the products contained in the basket. Given a basket, we compute the cosine similarities between its representation and all potential products, and pick top N-similar products. [[pdf]](https://astro.temple.edu/~tuc17157/pdfs/grbovic2015kddB.pdf), [[python]](https://github.com/lecheng/deeplearner)

4. doc2vec : a model for learning text representations. We apply doc2vec to obtain the product
representations from their titles. A basket’s representation is calculated as the mean of the products contained in it. Given a basket, we calculate the cosine similarities between the basket’s representation and all potential products, and pick top-N similar products. [[pdf]](https://arxiv.org/abs/1405.4053), [[python]](https://github.com/jhlau/doc2vec)

5. BPR-MF:  It optimizes the matrix factorization in a pairwise manner with Bayesian Personalized Ranking loss, which aims to maximize the difference between positive and negative items. It does not model the sequential signals. [[pdf]](https://arxiv.org/pdf/1205.2618.pdf), [[python]](https://github.com/caserec/CaseRecommender), [[python-2]](https://github.com/chenghu17/Sequential_Recommendation)

6. FMC: is is a simplified version of factorized personalized Markov Chain (FPMC) which does not include user personalized behaviours.

7. FPMC : is approach combines matrix factorization machine with Markov Chain for next item recommendations. The proposed approach captures both user-item preferences and user sequential behaviours. [[pdf]](https://www.ismll.uni-hildesheim.de/pub/pdfs/RendleFreudenthaler2010-FPMC.pdf), [[python]](https://github.com/flaviovdf/fpmc), [[python-2]](https://github.com/chenghu17/Sequential_Recommendation)

8. HRM : It is a Hierarchical Representation Model which captures both sequential and general user tastes by introducing both linear and nonlinear pooling operation for historical transaction aggregation. Here, the average aggregation is adopted.[[pdf]](http://www.bigdatalab.ac.cn/~junxu/publications/SIGIR2015_NextBasketRec.pdf), [[python]](https://github.com/chenghu17/Sequential_Recommendation)

9. PRME : This is model was originally proposed for POI recommendation. It utilizes metric embedding to learn user and item embeddings as well as the user check-in sequences. [[pdf]](https://pdfs.semanticscholar.org/d0ca/f22825647365a86ae4bf8749cfbe48789a8c.pdf), [[python]](https://github.com/flaviovdf/prme)

10. TransRec : This model applies the idea of translating embeddings to sequential recommendation. It views users as relation vectors and assumes that the next item is determined by user’s recent interacted item plus the user relation vectors. [[pdf]](https://dl.acm.org/citation.cfm?id=3109882), [[c++]](https://drive.google.com/file/d/0B9Ck8jw-TZUEVmdROWZKTy1fcEE/view)

11. TransFM : This model combines translation and metricbased approaches for sequential recommendation with Factorization Machines. [[pdf]](http://cseweb.ucsd.edu/~jmcauley/pdfs/recsys18a.pdf), [[python]](https://github.com/rpasricha/TransFM)

11. Caser : It models user past historical interactions with both hierarchical and vertical convolutional neural networks. It also considers the skip behaviors and the whole network is optimized by minimizing the cross entropy. [[pdf]](http://www.sfu.ca/~jiaxit/resources/wsdm18caser.pdf), [[matlab]](https://github.com/graytowne/caser)

11. SHAN : Sequential Recommender System based on Hierarchical Attention Network [[pdf]](https://www.ijcai.org/proceedings/2018/0546.pdf), [[python]](https://github.com/chenghu17/Sequential_Recommendation)

12. STAMP : Short-Term Attention/Memory Priority Model for Session-based Recommendation. [[pdf]](https://dl.acm.org/ft_gateway.cfm?id=3219950&type=pdf),[[python]](https://github.com/chenghu17/Sequential_Recommendation)

13. AttRec : This model combines self-attention and metric learning at the same time, is a sequence-based reommendation system algorithm. [[pdf]](https://arxiv.org/abs/1808.06414)

14. BASTEXT : a model of texts and shopping basket data, uses the texts for addressing the cold-start problem and uses the basket data for improving the performance of text representations. [[pdf]](https://arxiv.org/abs/1811.01166)

### Reference:
The the above information is taken from paper link or github below,

[(Paper) Learning Representations from Product Titles for Modeling Large-scale Transaction Logs](https://arxiv.org/abs/1811.01166) <br>
[(Paper) Next Item Recommendation with Self-Attention](https://arxiv.org/abs/1808.06414) <br>

---

[(Github) Case Recommender - A Python Framework for RecSys](https://github.com/caserec/CaseRecommender) <br>
[(Github deeplearner)](https://github.com/lecheng/deeplearner) <br>
[(Github) doc2vec](https://github.com/jhlau/doc2vec) <br>
[(Github) prod2vec](https://github.com/lecheng/deeplearner) <br>
[(Github) FPMC](https://github.com/flaviovdf/fpmc) <br>
[(Github) Sequential_Recommendation](https://github.com/chenghu17/Sequential_Recommendation) <br>
[(Github) TransFM](https://github.com/rpasricha/TransFM) <br>
[(Github) Caser](https://github.com/graytowne/caser) <br>
[(Github) PRME](https://github.com/flaviovdf/prme) <br>
