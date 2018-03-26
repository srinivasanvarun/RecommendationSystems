# RecommendationSystems
This repository contains python implementation of collaborative filtering recommendation systems. The following techniques are used:
  * User based CF - Cosine Similarity
  * User based CF - Pearson Correlation
  * User based CF - Pearson Correlation with Inverse user Frequency
  * User based CF - Pearson Correlation with Case modification
  * Item based CF - Modified Cosine Similarity
  * Ensemble Learning combining User based CF and Item based CF

## Files details
```
  --- Collaborative_CosineSimilarity.ipynb
  --- Collaborative_PearsonCorrelation.ipynb
  --- Collaborative_PearsonCorrelation-IUF.ipynb
  --- Collaborative_PearsonCorrelation-CaseAmplifaication.ipynb
  --- ItemCollaborative_AdjustedCosineSimilarity.ipynb
  --- EnsembleLearning.ipynb
  --- traindata
    +--- train.txt
  --- testdata
    +--- test5.txt
    +--- test10.txt
    +--- test20.txt
  --- train_ensemble
    +--- test5_1.txt
    +--- test5_2.txt
    +--- test10_1.txt
    +--- test10_2.txt
    +--- test20_1.txt
    +--- test20_2.txt
  --- output
    +--- test5.txt
    +--- test10.txt
    +--- test20.txt
```
## Results
| Collaborative filtering Method | RSME (Given 5 ratings) | RSME (Given 10 ratings) | RSME (Given 20 ratings) | RSME Average |
| --- | --- | --- | --- | --- |
| `User based - Cosine Similarity` | 0.787 | 0.78 | 0.756 | 0.772 |
| `User based - Pearson Method` | 0.833 | 0.784 | 0.77 | 0.794 |
| `User based - Pearson Method with Inverse User Frequency` | 1.035 | 0.94 | 0.963 | 0.981 |
| `User based - Pearson Method with Case Modification` | 0.856 | 0.766 | 0.777 | 0.801 |
| `Item based - Modified Cosine Similarity` | 0.992 | 0.952 | 0.92 | 0.952 |
| `Ensemble Learning (User & item-based CF)` | 0.904 | 0.836 | 0.844 | 0.862 |
