
* Utilized the **Breast Cancer Diagnosis** dataset.
* Encoded the `diagnosis` column as numerical values for classification.
* Split the dataset into training and testing sets using `train_test_split`.
* Applied **standard scaling** to normalize the features.
* Built and trained a **Linear SVM model**, achieving the following confusion matrix:

  ```
  [[68,  3],
   [ 2, 41]]
  ```

  * Weighted average recall: **0.96**.
* Built and trained an **RBF SVM model**, achieving the following confusion matrix:

  ```
  [[71,  0],
   [ 2, 41]]
  ```

  * Weighted average recall: **0.98**.
* Applied **Principal Component Analysis (PCA)** to project the dataset into 2D space for visualization.

  * Used PCA’s `inverse_transform` method to map the mesh grid points back into the original feature space for decision boundary evaluation.
  * Used the **decision function** values to plot the decision boundaries in PCA space.
  * The RBF model produced a **curved boundary**, illustrating its non-linear decision surface.
* Performed **GridSearchCV** to optimize the `C` and `gamma` hyperparameters, using **recall** as the scoring metric.

  * Conducted optimization separately for both the linear and RBF models.
  * Plotted the new decision boundaries for each optimized model.

