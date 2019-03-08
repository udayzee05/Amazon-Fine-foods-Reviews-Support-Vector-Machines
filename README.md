# Amazon-Fine-foods-Reviews-Support-Vector-Machines

Applying SVM on these feature sets • SET 1:Review text, preprocessed one converted into vectors using (BOW)
• SET 2:Review text, preprocessed one converted into vectors using (TFIDF)
• SET 3:Review text, preprocessed one converted into vectors using (AVG W2v)
• SET 4:Review text, preprocessed one converted into vectors using (TFIDF W2v)
Procedure
• We will work with 2 versions of SVM
 Linear kernel
 RBF kernel
• While working with linear kernel, used SGDClassifier’ with hinge loss because it is computationally less expensive.
• While working with ‘SGDClassifier’ with hinge loss and trying to find the AUC score, used CalibratedClassifierCV
• Similarly, like kdtree of knn, While working with RBF kernel it's better to reduce the number of dimensions. We used min_df = 10, max_features = 500 and consider a sample size of 40k points.
