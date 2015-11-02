# Predict if salary is >50k with machine learning

A neural network with two layers (sigmoid activation) is used to predict if someone makes more than 50k or less based on training and test data from the UCI Machine Learning Repository.

Percentage right: 85.333% on 16281 test entries on which we did not trained the neural network.
Therefore, the error is of 14.667%.


## Dependencies

- Python 3.0 (Anaconda distribution is preferred),
- Theano (requires linux),
- Keras (requires Theano),
- iPython notebook (included in Anaconda bundle, run `ipython notebook` in terminal from the project's directory).


## Comparison with other regression methods on the dataset

__Algorithm__              | __Error (%)__
----------------       | ---------
__My neural network__  | __14.67__
C4.5                   | 15.54
C4.5-auto              | 14.46
C4.5 rules             | 14.94
Voted ID3 (0.6)        | 15.64
Voted ID3 (0.8)        | 16.47
T2                     | 16.84
1R                     | 19.54
NBTree                 | 14.10
CN2                    | 16.00
HOODG                  | 14.82
FSS Naive Bayes        | 14.05
IDTM (Decision table)  | 14.46
Naive-Bayes            | 16.12
Nearest-neighbor (1)   | 21.42
Nearest-neighbor (3)   | 20.35
OC1                    | 15.04
Pebls                  | Crashed.


## Dataset's structure

### 2 Outputs (classification)
- &gt;50K,
- &lt;=50K.

### 14 Inputs (string and continuous)
- age: continuous.
- workclass: Private, Self-emp-not-inc, Self-emp-inc, Federal-gov, Local-gov, State-gov, Without-pay, Never-worked.
- fnlwgt: continuous.
- education: Bachelors, Some-college, 11th, HS-grad, Prof-school, Assoc-acdm, Assoc-voc, 9th, 7th-8th, 12th, Masters, 1st-4th, 10th, Doctorate, 5th-6th, Preschool.
- education-num: continuous.
- marital-status: Married-civ-spouse, Divorced, Never-married, Separated, Widowed, Married-spouse-absent, Married-AF-spouse.
- occupation: Tech-support, Craft-repair, Other-service, Sales, Exec-managerial, Prof-specialty, Handlers-cleaners, Machine-op-inspct, Adm-clerical, Farming-fishing, Transport-moving, Priv-house-serv, Protective-serv, Armed-Forces.
- relationship: Wife, Own-child, Husband, Not-in-family, Other-relative, Unmarried.
- race: White, Asian-Pac-Islander, Amer-Indian-Eskimo, Other, Black.
- sex: Female, Male.
- capital-gain: continuous.
- capital-loss: continuous.
- hours-per-week: continuous.
- native-country: United-States, Cambodia, England, Puerto-Rico, Canada, Germany, Outlying-US(Guam-USVI-etc), India, Japan, Greece, South, China, Cuba, Iran, Honduras, Philippines, Italy, Poland, Jamaica, Vietnam, Mexico, Portugal, Ireland, France, Dominican-Republic, Laos, Ecuador, Taiwan, Haiti, Columbia, Hungary, Guatemala, Nicaragua, Scotland, Thailand, Yugoslavia, El-Salvador, Trinadad&Tobago, Peru, Hong, Holand-Netherlands.

_Note: some data contain "?", so this value is possible for each of those 14 input fields_


## Presentation's slides

The slides of the seminar are available [here](https://docs.google.com/presentation/d/1Ynz-IN8iMyD1Fp1gqUuX5_0SOxSUhS1LFzO_bB9Di68/present?usp=sharing) (in French).



## References

[Dataset infos](http://archive.ics.uci.edu/ml/datasets/Adult)

Source:
> Lichman, M. (2013). UCI Machine Learning Repository [http://archive.ics.uci.edu/ml]. Irvine, CA: University of California, School of Information and Computer Science.
