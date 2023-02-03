---
{"dg-publish":true,"permalink":"/books/highlights/2019-the-hundred-page-machine-learning-book-andriy-burkov/"}
---

# The Hundred-Page Machine Learning Book-Andriy Burkov
## Metadata
* Author: [[2019\|2019]]

## Highlights
models are wrong, but some are useful.” — George Box The book is distributed on the “read frst, buy later” principle. Andriy Burkov The Hundred-Page Machine Learning Book - Draft — location: []()
{ #ref-27704}


---
“All models are wrong, but some are useful.” — George Box — location: []()
{ #ref-40789}


---
The algorithm I use to illustrate supervised learning is called Support Vector Machine (SVM). This algorithm requires that the positive label (in our case it’s “spam”) has the numeric value of +1 (one), and the negative label (“not_spam”) has the value of ≠1 (minus one) — location: []()
{ #ref-4813}


---
We would also prefer that the hyperplane separates positive examples from negative ones with the largest margin. The margin is the distance between the closest examples of two classes, as defned by the decision boundary. A large margin contributes to a better generalization, that is how well the model will classify new examples in the future. To achieve that, we need to minimize the Euclidean norm of w denoted by ÎwÎ and given by ÒqD j=1(w(j))2 — location: []()
{ #ref-4049}


---
3 Fundamental Algorithms — location: []()
{ #ref-57669}


---
3.1 Linear Regression — location: []()
{ #ref-38037}


---
3.2 Logistic Regression — location: []()
{ #ref-28026}


---
The frst thing to say is that logistic regression is not a regression, but a classifcation learning algorithm. The name comes from statistics and is due to the fact that the mathematical formulation of logistic regression is similar to that of linear regression. I explain logistic regression on the case of binary classifcation.However, it can naturally be extended to multiclass classifcation — location: []()
{ #ref-23379}


---
3.3 Decision Tree Learning — location: []()
{ #ref-56907}


---
A decision tree is an acyclic graph that can be used to make decisions. In each branching node of the graph, a specifc feature j of the feature vector is examined. If the value of the feature is below a specifc threshold, then the left branch is followed; otherwise, the right branch is followed. As the leaf node is reached, the decision is made about the class to which the example belongs — location: []()
{ #ref-1391}


---
3.4 Support Vector Machine — location: []()
{ #ref-51331}


---
3.5 k-Nearest Neighbors — location: []()
{ #ref-41257}


---
k-Nearest Neighbors (kNN) is a non-parametric learning algorithm. Contrary to other learning algorithms that allow discarding the training data after the model is built, kNN keeps all training examples in memory. Once a new, previously unseen example x comes in, the kNN algorithm fnds k training examples closest to x and returns the majority label (in case of classifcation) or the average label (in case of regression — location: []()
{ #ref-64126}


---
SVMs that optimize hinge loss are called soft-margin SVMs, while the original formulation is referred to as a hard-margin SVM — location: []()
{ #ref-20608}


---
CÎwÎ2 + max (0, 1 ≠ yi(wxi ≠ b)) , 3.4.1 Dealing with Noise To extend SVM to cases in which the data is not linearly separable, we introduce the hinge loss function: max (0, 1 ≠ yi(wxi ≠ b)). The hinge loss function is zero if the constraints a) and b) are satisfed, in other words, if wxi lies on the correct side of the decision boundary. For data on the wrong side of the decision boundary, the function’s value is proportional to the distance from the decision boundary. We — location: []()
{ #ref-63055}


---
