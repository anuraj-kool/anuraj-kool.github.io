- resources
	- rules of ml: https://martin.zinkevich.org/rules_of_ml/rules_of_ml.pdf
	- ml interviews: https://www.educative.io/courses/grokking-the-machine-learning-interview
	- designing machine learning systems: https://github.com/chiphuyen/dmls-book
	- mlops: https://github.com/chiphuyen/dmls-book/blob/main/mlops-tools.md
	- interpretibility: https://christophm.github.io/interpretable-ml-book/interpretability.html
	- requirements checklist: https://twolodzko.github.io/posts/ml-checklist.html
- concepts
	- ml system requirements
		- reliability
		- scalability
		- maintainability
		- adaptability
	- task types
		- classification
			- binary
			- multiclass
				- use cross entropy loss
				- heirarchial classification
			- multilabel
				- cross entropy loss
				- one model per label
				- use each label as feature instead
	- objective functions
		- rsme #card [[ml flashcards]]
		  card-last-interval:: 4
		  card-repeats:: 1
		  card-ease-factor:: 2.36
		  card-next-schedule:: 2024-10-09T04:19:36.830Z
		  card-last-reviewed:: 2024-10-05T04:19:36.830Z
		  card-last-score:: 3
			- ```
			  ```
		- def cross_entropy(labels, predictions) #card [[ml flashcards]]
		  card-last-score:: 3
		  card-repeats:: 1
		  card-next-schedule:: 2024-10-09T04:19:32.692Z
		  card-last-interval:: 4
		  card-ease-factor:: 2.36
		  card-last-reviewed:: 2024-10-05T04:19:32.692Z
			- ```
			  - sum([labels[p_i] * np.log(predictions[p_i]) for p_i in range(predictions)])
			  ```
		- logistic loss #card
		  card-last-interval:: 4
		  card-repeats:: 1
		  card-ease-factor:: 2.6
		  card-next-schedule:: 2024-10-09T04:20:26.592Z
		  card-last-reviewed:: 2024-10-05T04:20:26.593Z
		  card-last-score:: 5
		- combining objective functions
			- weighted averages of loss ``alpha * loss_1 + beta * loss_2``
			- weighted averages of scores ``alpha * score_1 + beta * score_2``
	- training data
		- sampling
			- ``def weighted_sample(items: List[Any], weights: List[float], k: int = 1) -> List[Any]:`` #card [[ml flashcards]]
			- ``def stratified_sample_np(X, y, test_size=0.2, random_state=None):`` #card [[ml flashcards]]
			- ``def reservior_sample()`` #card [[ml flashcards]]
		- class imbalance
			- use right eval metrics
				- precision = tp/tp+fp
				- (true positive rate) recall = tp/tp+fn
				- (false positive rate) = fp/tn + fp
				- f1 = 2 * precision * recall / (precision + recall)
					- The F1 score is highest when precision and recall are balanced.
				- roc curve - pick a probability threshold which maximizes recall and minimizes false positive rate
				- precision-recall curve - staircase
					- ``ap (average precision) = sum (precision[i] * recall[i] - recall[i -1] for i in range(thresholds))``
				- Which is better for class imbalance?
					- [precision-recall curves](https://scikit-learn.org/stable/auto_examples/model_selection/plot_precision_recall.html) are generally better for imbalanced datasets, especially when you're more interested in the minority class
					- focus on minority class: in imbalanced datasets, we're often more interested in correctly identifying the minority class. Precision-Recall curves focus on this directly.
					- sensitivity to changes: In imbalanced datasets, a large change in the number of false positives might lead to a small change in FPR (used in ROC) but a large change in Precision.
					- avoiding misleading results: ROC curves can present an overly optimistic view of performance on imbalanced datasets. A model can have a high AUC (Area Under the Curve) for ROC even if it performs poorly on the minority class.
					- threshold selection: When choosing a threshold for classification, Precision-Recall curves can give you a clearer picture of the trade-offs you're making in terms of precision and recall for the minority class.
					- choose ROC for balanced dataset when focus is on avoiding false positives while improving tp (accuracy)
			- customize loss function based on sample weight
				- learner tries to optimize for samples with high loss
				- cost sensitive learning
					- confusion matrix but for cost
					- loss becomes weighted sum of p * (cij * pj) for j in diff classes
				- class balanced loss
		- eda
			- pdp
			- pearson correlation
			- scatterplot
	- feature engineering
		- scaling
			- min/max scaling ``x' = x - min(x) / max(x) - min(x)``
			- range based min/max scaling ``x'' = a + (b-a) * x'``
			- standard scaling ``x' = x-xm/std``
			- log scaling for skewed features to make it normal
				- prone to leakage
				- global stats
			- discrete bins
		- hashing to 2^n and treating as categorical
			- collisions but okay
		- feature crossing
		- feature derivations
		- embeddings
			- word embeddings
			- positions embeddings
				- can be learnt
				- can be predefined as sine, cosine for different positions, even, odd pos
					- works great for coordinate features
		- tfidf, tf, feature hashing for text
		- data leakage
			- incorrect splits
				- folds
				- leakage from validation/test
					- scaling before split
					- missing data from test
				- duplicates
				- finetuning hyperparams on test split
		- feature selection
			- lasso/L1
		- feature importance
			- shap
				- attributes contribution of features for a given point to difference between average prediction (mean) and current prediction
			- tree based
			- coefficient of LR
		-
			-
-
	-
	- metrics
		- supervised
			- logloss
			- rmse
			- confusion metric
			- precision/recall
		- unsupervised
			- ndcg
			- precision/recall at k
	- feature engineering
		- normalization
		- one hot encoding
		- target encoding
		- embeddings
	- feature selection
		- leave one out
		- weights
		- feature importance
	- interpretability
		- pertubation
		- smote
	- errors
	- a/b testing
	- data lineage, skew
	- quantization
- tools
  collapsed:: true
	- onnyx
	- accelerate