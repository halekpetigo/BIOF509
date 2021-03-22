# BIOF509 Final Project

Can heart attacks be predicted? This project attempts to answer that using machine learning algorithms? This project first implements 3 unsupervised learning algorithms (K-Means, density based clustering, and hierarchical clustering) to group the studied population into observable clusters. Then 3 supervised learning algorithms (SVM, Decision Tree and Bayesian) are used to predict at risk patients. The implemented algorithms efficiency are compared.

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

### Prerequisites

This tool uses numpy, pandas, seaborn, umap, matplotlib and sklearn. If you do not have all the needed libraries to run the project, please install using pip install. 

```
pip install missing_library

example to install seaborn
pip install seaborn
```

### Getting latest version of the tool on your local environment

Step by step instruction on how to get a development env running

Clone project on your local machine.

```
git clone https://github.com/halekpetigo/BIOF509
```

Open FAES-BIOF-509-Hale_Kpetigo-FinalProject.ipynb with Jupyter Lab.

There are two classes in the tool. BIOF509Unsupervised and BIOF509Supervised. 

BIOF509Unsupervised is used to analyze and classify the two example datasets provided.
BIOF509Supervised is used to analyze and classify the two example datasets provided.

The two datasets provided are heart.csv and heart 2.csv. heart.csv is the complete Heart Disease Dataset from the University of California, Irvine. It contains 1025 records of patients from Cleveland, Hungarian, Switzerland and Long Beach VA. heart 2.csv contains 303 records which are the dataset from Cleveland.

BIOF509Unsupervised has four main methods.
- data_analysis: Used to provide general analysis of the dataset
- BIOF509Kmeans: Used to classify data using K-Means
- BIOF509Density: Used to classify data using Density clustering
- BIOF509Hierarchical: Used to classify data using Hierarchical Clustering

BIOF509Supervised has three main methods.
- BIOF509SVM: Used to predict using SVM
- BIOFDecisionTree: Used to predict using Decision Tree
- BIOFBayesian: Used to predict using Gaussian Naive Bayes

* **BIOF509Unsupervised**

Running BIOF509Unsupervised data_analysis. Play Cell 2 and Cell 3. In Cell 4 run the code below

```
# Load Cleveland only dataset
FinalProject = BIOF509Unsupervised("heart 2.csv")
# Second dataset used for comparision. Uncomment to use whole 1025 dataset
# FinalProject = BIOF509Unsupervised("heart.csv")
FinalProject.data_analysis()

```

Running BIOF509Unsupervised BIOF509Kmeans. Play Cell 2 and Cell 3. In Cell 4 run the code below

```
# Load Cleveland only dataset
FinalProject = BIOF509Unsupervised("heart 2.csv")
# Second dataset used for comparision. Uncomment to use whole 1025 dataset
# FinalProject = BIOF509Unsupervised("heart.csv")

FinalProject.BIOF509Kmeans()
```

Running BIOF509Unsupervised BIOF509Density. Play Cell 2 and Cell 3. In Cell 4 run the code below

```
# Load Cleveland only dataset
FinalProject = BIOF509Unsupervised("heart 2.csv")
# Second dataset used for comparision. Uncomment to use whole 1025 dataset
# FinalProject = BIOF509Unsupervised("heart.csv")

FinalProject.BIOF509Density()
```

Running BIOF509Unsupervised BIOF509Hierarchical. Play Cell 2 and Cell 3. In Cell 4 run the code below

```
# Load Cleveland only dataset
FinalProject = BIOF509Unsupervised("heart 2.csv")
# Second dataset used for comparision. Uncomment to use whole 1025 dataset
# FinalProject = BIOF509Unsupervised("heart.csv")

FinalProject.BIOF509Hierarchical()
```

* **BIOF509Supervised**

Running BIOF509Supervised BIOF509SVM. Play Cell 2 and Cell 5. In Cell 20 run the code below

```
# Load Cleveland only dataset
FinalSupProject = BIOF509Supervised("heart 2.csv")
# Second dataset used for comparision. Uncomment to use whole 1025 dataset
#FinalSupProject = BIOF509Supervised("heart.csv")

FinalSupProject.BIOF509SVM()
```

Running BIOF509Supervised BIOFDecisionTree. Play Cell 2 and Cell 5. In Cell 20 run the code below

```
# Load Cleveland only dataset
FinalSupProject = BIOF509Supervised("heart 2.csv")
# Second dataset used for comparision. Uncomment to use whole 1025 dataset
#FinalSupProject = BIOF509Supervised("heart.csv")

FinalSupProject.BIOFDecisionTree()
```

Running BIOF509Supervised BIOFBayesian. Play Cell 2 and Cell 5. In Cell 20 run the code below

```
# Load Cleveland only dataset
FinalSupProject = BIOF509Supervised("heart 2.csv")
# Second dataset used for comparision. Uncomment to use whole 1025 dataset
#FinalSupProject = BIOF509Supervised("heart.csv")

FinalSupProject.BIOFBayesian()
```


## Built With

* [Jupyter Lab](https://jupyterlab.readthedocs.io/en/latest/) - The data science IED used
* [Anaconda](https://docs.anaconda.com/) - Python Environment Manager


## Datasets

* [UCI Heart Disease Dataset](https://archive.ics.uci.edu/ml/datasets/heart+disease)
* [Cleveland only dataset](https://www.kaggle.com/nareshbhat/health-care-data-set-on-heart-attack-possibility)
* [Complete dataset](https://www.kaggle.com/johnsmith88/heart-disease-dataset)


## Authors

* **Hale Kpetigo** - [Github Repo](https://github.com/halekpetigo)


## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details

## Acknowledgments

* Special thanks to James Anibal and Christina
