Dirichlet-Multinomial Bayes Classifier (DMBC) for Microbiome Classification
---------------------------------------------------------------------------
This package implements the machine-learning method described by Gao et al (2016) for microbiome classification using a Bayes classifier based on the Dirichlet-Multinomial distribution.  In addition to classification, the package also identifies a subset of microbial taxa that can achieve the maximum classification accuracy.

## Installation

* Make sure you have **_R >= 3.2.0_**.
* Make sure you have **devtools** installed and do the following:
```R
library(devtools)
install_github("qunfengdong/DMBC")
```

## Usage

There are totally 6 functions included in the package. The most important one is **dmbc_predict**, which will predict probability for a test set from DMBC model given a training set.

1. **best_cm**: Confusion Matrix for the Best Model
2. **CalPrb**: Calculate Likelihood based on Dirichlet-multinomial distribution estimated parameters
3. **Cal_AUC**: Calculate Area Under the ROC Curve from Leave-One-Out Cross-Validation
4. **dmbc_predict**: Predict probability from DMBC model
5. **FS**: Filter and Feature Selection based on Wilcoxon Rank-Sum test
6. **loocv**: Leave one out cross-validation

Example data sets:
* *_test_*: Example Testing Data
* *_training_*: Example Training Data

## Contributors

* Xiang Gao (Author)
* Qunfeng Dong (Author)
* Huaiying Lin (Maintainer)

## License

MIT
