Class imbalance is common in many real-world applications of binary classification, such as rare disease screening, fraud detection, loan default prediction, 
and law enforcement (e.g., predicting illegal content in air/sea cargo), amongst others. It occurs when one category (for example, negative) is much more 
frequent than the other (for example, positive). Consider fraudulent credit-card transactions - the positive class (fraud) may represent less than 0.1% of 
the data. In such cases, classifiers tend to favour the majority class, often achieving high overall accuracy simply by predicting it most of the time.
One technique used to address this problem is to either oversample the minority class or downsample the majority class. Oversampling rebalances the data 
by randomly duplicating minority-class samples, whereas downsampling randomly removes a portion of the majority-class samples.

In this notebook we use a simple synthetic dataset example to compare different resampling strategies and show how they affect prediction accuracy in a 
binary classification task. We will point out some common pitfalls to watch for when applying these techniques and evaluating their results.
