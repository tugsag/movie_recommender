# Various attempts at making a movie recommender system
Different approaches are taken. Small movielens dataset for ncf and ranking_and_mf files. tmdb datasets for the content_filtering file. This repo is meant to be practice and as a launch point for others looking to get started with recommendation systems.


ncf.ipynb involves DL based appraoches where an embedding is learned. Requires **tensorflow-keras** and **recommendations** libraries. Some work better than others. Examples referenced from documentations and github pages of libraries.

ranking_and_mf.ipynb involves using the **surprise** library to do matrix factorization. Ranking (requires **lightgbm** library) and regression (requires **sklearn**) attempts are made as well. MF appraoch seems to work the best using surprise.

content_filtering.ipynb invovles using content descriptions to recommend like movies. We can further use this by picking the top rated movies for the user in question and using content filtering to suggest like items. A short intro to MF is introduced using **surprise** SVD at the end. Will take a long time to run due to sheer size of dataset. Otherwise, only using content information runs fairly quickly.

wnd.ipynb implements Wide and Deep network structure to predict movielens data. credit: https://wngaw.github.io/wide-and-deep-learning/