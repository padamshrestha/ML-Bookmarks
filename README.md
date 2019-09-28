# ML-ResourceNote
 
## About
We expose our online track public. Here, we share some of our attention space .... This is our personal tracking repo, so contents her may be updated frequently based on our interest in the field of Machine Learning and Data Science. 



## Table of Contents
- [GitHub Geeks](#github-geeks)
- [Data Set Collection](#data-set)
- [Book Materials](#book-materials)
  * [Contact](#contact)

## Book Materials
* Machine Learning 
   + [Hands-On Machine Learning with Scikit-Learn and TensorFlow: Concepts, Tools, and Techniques to Build Intelligent Systems](https://www.amazon.com/Hands-Machine-Learning-Scikit-Learn-TensorFlow/dp/1491962291)
   + [Python Machine Learning](https://www.amazon.com/Python-Machine-Learning-Sebastian-Raschka-ebook/dp/B00YSILNL0)
   + [The Hundred-Page Machine Learning Book](https://www.amazon.com/Hundred-Page-Machine-Learning-Book/dp/199957950X)
* Deep Learning 
  + [Deep Learning](https://www.deeplearningbook.org/) 
  + [Deep Learning with Python](https://www.amazon.com/Deep-Learning-Python-Francois-Chollet/dp/1617294438)
  + [Deep Learning for Computer Vision with Python](https://www.pyimagesearch.com/deep-learning-computer-vision-python-book/)
  + [Reinforcement Learning: An Introduction](https://www.amazon.com/Reinforcement-Learning-Introduction-Adaptive-Computation-ebook/dp/B008H5Q8VA)
* Big Data
  + [Data Mining: Concepts and Techniques](https://www.amazon.com/Data-Mining-Concepts-Techniques-Management/dp/0123814790)
  + [An Introduction to Statistical Learning: with Applications in R](https://www.amazon.com/Introduction-Statistical-Learning-Applications-Statistics/dp/1461471370)
  + [Python for Data Analysis](https://www.amazon.com/Python-Data-Analysis-Wrangling-IPython-ebook/dp/B075X4LT6K)
  + [Learning Spark: Lightning-Fast Big Data Analysis](https://www.amazon.com/Learning-Spark-Lightning-Fast-Data-Analysis/dp/1449358624)
  + [High Performance Spark: Best Practices for Scaling and Optimizing Apache Spark](https://www.amazon.com/High-Performance-Spark-Practices-Optimizing/dp/1491943203)


## Data Set
* [Google Dataset Search](https://toolbox.google.com/datasetsearch)
* [Kaggle](https://www.kaggle.com/datasets)
* [UCI Machine Learning Repository](http://mlr.cs.umass.edu/ml/)
* [Academic Torrent](http://academictorrents.com/browse.php?cat=6)

## GitHub Geeks
We include a very few amount of our favorite GitHub Geeks. 

|       GitHub Profile            | Point of Interest  | Interested Projects |
|-------------------|-------|-------|
|[Ian Goodfellow](https://github.com/goodfeli)        |ML Expert  |[GAN](https://github.com/goodfeli/adversarial) |
|[Michael Nielsen](https://github.com/mnielsen)             |ML Expert   |[Neural Networks and Deep Learning](https://github.com/mnielsen/neural-networks-and-deep-learning) |
|[Grant Sanderson](https://github.com/3b1b)          |Math Expert  |[Animation Engin for Math](https://github.com/3b1b/manim) |
|[Matthijs Hollemans](https://github.com/hollance)       |ML Expert   |[Forge](https://github.com/hollance/Forge) |
|[Andrej](https://github.com/karpathy)      |ML Expert   |[ReinforceJs](https://github.com/karpathy/reinforcejs) |
|[Alex J. Champandard](https://github.com/alexjc)              |ML Expert   |[Neural-Doodle](https://github.com/alexjc/neural-doodle) |
|[Piotr Migdał](https://github.com/stared)          |ML Expert   |[Quantum-Game](https://github.com/stared/quantum-game) |
|[Reiichiro Nakano](https://github.com/reiinakano)           |ML Expert   |[Xcessiv](https://github.com/reiinakano/xcessiv) |
|[Zhuang Liu](https://github.com/liuzhuang13) |ML Expert  |[DenseNet](https://github.com/liuzhuang13/DenseNet) |
|[Bolei Zhou](https://github.com/metalbubble?fbclid=IwAR29k07i9Vjs9Ay6ZXr4ZNLc0Wln-6ha6xAHXMs5K7OBqgkXlPxAZ7_jH0Y)       |ML Expert  |[CAM](https://github.com/metalbubble/CAM) |



## Installation
    $ git clone https://github.com/eriklindernoren/ML-From-Scratch
    $ cd ML-From-Scratch
    $ python setup.py install

## Examples
### Polynomial Regression
    $ python mlfromscratch/examples/polynomial_regression.py

<p align="center">
    <img src="http://eriklindernoren.se/images/p_reg.gif" width="640"\>
</p>
<p align="center">
    Figure: Training progress of a regularized polynomial regression model fitting <br>
    temperature data measured in Linköping, Sweden 2016.
</p>

### Classification With CNN
    $ python mlfromscratch/examples/convolutional_neural_network.py

    +---------+
    | ConvNet |
    +---------+
    Input Shape: (1, 8, 8)
    +----------------------+------------+--------------+
    | Layer Type           | Parameters | Output Shape |
    +----------------------+------------+--------------+
    | Conv2D               | 160        | (16, 8, 8)   |
    | Activation (ReLU)    | 0          | (16, 8, 8)   |
    | Dropout              | 0          | (16, 8, 8)   |
    | BatchNormalization   | 2048       | (16, 8, 8)   |
    | Conv2D               | 4640       | (32, 8, 8)   |
    | Activation (ReLU)    | 0          | (32, 8, 8)   |
    | Dropout              | 0          | (32, 8, 8)   |
    | BatchNormalization   | 4096       | (32, 8, 8)   |
    | Flatten              | 0          | (2048,)      |
    | Dense                | 524544     | (256,)       |
    | Activation (ReLU)    | 0          | (256,)       |
    | Dropout              | 0          | (256,)       |
    | BatchNormalization   | 512        | (256,)       |
    | Dense                | 2570       | (10,)        |
    | Activation (Softmax) | 0          | (10,)        |
    +----------------------+------------+--------------+
    Total Parameters: 538570

    Training: 100% [------------------------------------------------------------------------] Time: 0:01:55
    Accuracy: 0.987465181058

<p align="center">
    <img src="http://eriklindernoren.se/images/mlfs_cnn1.png" width="640">
</p>
<p align="center">
    Figure: Classification of the digit dataset using CNN.
</p>

### Density-Based Clustering
    $ python mlfromscratch/examples/dbscan.py

<p align="center">
    <img src="http://eriklindernoren.se/images/mlfs_dbscan.png" width="640">
</p>
<p align="center">
    Figure: Clustering of the moons dataset using DBSCAN.
</p>

### Generating Handwritten Digits
    $ python mlfromscratch/unsupervised_learning/generative_adversarial_network.py

    +-----------+
    | Generator |
    +-----------+
    Input Shape: (100,)
    +------------------------+------------+--------------+
    | Layer Type             | Parameters | Output Shape |
    +------------------------+------------+--------------+
    | Dense                  | 25856      | (256,)       |
    | Activation (LeakyReLU) | 0          | (256,)       |
    | BatchNormalization     | 512        | (256,)       |
    | Dense                  | 131584     | (512,)       |
    | Activation (LeakyReLU) | 0          | (512,)       |
    | BatchNormalization     | 1024       | (512,)       |
    | Dense                  | 525312     | (1024,)      |
    | Activation (LeakyReLU) | 0          | (1024,)      |
    | BatchNormalization     | 2048       | (1024,)      |
    | Dense                  | 803600     | (784,)       |
    | Activation (TanH)      | 0          | (784,)       |
    +------------------------+------------+--------------+
    Total Parameters: 1489936

    +---------------+
    | Discriminator |
    +---------------+
    Input Shape: (784,)
    +------------------------+------------+--------------+
    | Layer Type             | Parameters | Output Shape |
    +------------------------+------------+--------------+
    | Dense                  | 401920     | (512,)       |
    | Activation (LeakyReLU) | 0          | (512,)       |
    | Dropout                | 0          | (512,)       |
    | Dense                  | 131328     | (256,)       |
    | Activation (LeakyReLU) | 0          | (256,)       |
    | Dropout                | 0          | (256,)       |
    | Dense                  | 514        | (2,)         |
    | Activation (Softmax)   | 0          | (2,)         |
    +------------------------+------------+--------------+
    Total Parameters: 533762


<p align="center">
    <img src="http://eriklindernoren.se/images/gan_mnist5.gif" width="640">
</p>
<p align="center">
    Figure: Training progress of a Generative Adversarial Network generating <br>
    handwritten digits.
</p>

### Deep Reinforcement Learning
    $ python mlfromscratch/examples/deep_q_network.py

    +----------------+
    | Deep Q-Network |
    +----------------+
    Input Shape: (4,)
    +-------------------+------------+--------------+
    | Layer Type        | Parameters | Output Shape |
    +-------------------+------------+--------------+
    | Dense             | 320        | (64,)        |
    | Activation (ReLU) | 0          | (64,)        |
    | Dense             | 130        | (2,)         |
    +-------------------+------------+--------------+
    Total Parameters: 450

<p align="center">
    <img src="http://eriklindernoren.se/images/mlfs_dql1.gif" width="640">
</p>
<p align="center">
    Figure: Deep Q-Network solution to the CartPole-v1 environment in OpenAI gym.
</p>

### Image Reconstruction With RBM
    $ python mlfromscratch/examples/restricted_boltzmann_machine.py

<p align="center">
    <img src="http://eriklindernoren.se/images/rbm_digits1.gif" width="640">
</p>
<p align="center">
    Figure: Shows how the network gets better during training at reconstructing <br>
    the digit 2 in the MNIST dataset.
</p>

### Evolutionary Evolved Neural Network
    $ python mlfromscratch/examples/neuroevolution.py

    +---------------+
    | Model Summary |
    +---------------+
    Input Shape: (64,)
    +----------------------+------------+--------------+
    | Layer Type           | Parameters | Output Shape |
    +----------------------+------------+--------------+
    | Dense                | 1040       | (16,)        |
    | Activation (ReLU)    | 0          | (16,)        |
    | Dense                | 170        | (10,)        |
    | Activation (Softmax) | 0          | (10,)        |
    +----------------------+------------+--------------+
    Total Parameters: 1210

    Population Size: 100
    Generations: 3000
    Mutation Rate: 0.01

    [0 Best Individual - Fitness: 3.08301, Accuracy: 10.5%]
    [1 Best Individual - Fitness: 3.08746, Accuracy: 12.0%]
    ...
    [2999 Best Individual - Fitness: 94.08513, Accuracy: 98.5%]
    Test set accuracy: 96.7%

<p align="center">
    <img src="http://eriklindernoren.se/images/evo_nn4.png" width="640">
</p>
<p align="center">
    Figure: Classification of the digit dataset by a neural network which has<br>
    been evolutionary evolved.
</p>

### Genetic Algorithm
    $ python mlfromscratch/examples/genetic_algorithm.py

    +--------+
    |   GA   |
    +--------+
    Description: Implementation of a Genetic Algorithm which aims to produce
    the user specified target string. This implementation calculates each
    candidate's fitness based on the alphabetical distance between the candidate
    and the target. A candidate is selected as a parent with probabilities proportional
    to the candidate's fitness. Reproduction is implemented as a single-point
    crossover between pairs of parents. Mutation is done by randomly assigning
    new characters with uniform probability.

    Parameters
    ----------
    Target String: 'Genetic Algorithm'
    Population Size: 100
    Mutation Rate: 0.05

    [0 Closest Candidate: 'CJqlJguPlqzvpoJmb', Fitness: 0.00]
    [1 Closest Candidate: 'MCxZxdr nlfiwwGEk', Fitness: 0.01]
    [2 Closest Candidate: 'MCxZxdm nlfiwwGcx', Fitness: 0.01]
    [3 Closest Candidate: 'SmdsAklMHn kBIwKn', Fitness: 0.01]
    [4 Closest Candidate: '  lotneaJOasWfu Z', Fitness: 0.01]
    ...
    [292 Closest Candidate: 'GeneticaAlgorithm', Fitness: 1.00]
    [293 Closest Candidate: 'GeneticaAlgorithm', Fitness: 1.00]
    [294 Answer: 'Genetic Algorithm']

### Association Analysis
    $ python mlfromscratch/examples/apriori.py
    +-------------+
    |   Apriori   |
    +-------------+
    Minimum Support: 0.25
    Minimum Confidence: 0.8
    Transactions:
        [1, 2, 3, 4]
        [1, 2, 4]
        [1, 2]
        [2, 3, 4]
        [2, 3]
        [3, 4]
        [2, 4]
    Frequent Itemsets:
        [1, 2, 3, 4, [1, 2], [1, 4], [2, 3], [2, 4], [3, 4], [1, 2, 4], [2, 3, 4]]
    Rules:
        1 -> 2 (support: 0.43, confidence: 1.0)
        4 -> 2 (support: 0.57, confidence: 0.8)
        [1, 4] -> 2 (support: 0.29, confidence: 1.0)


## Implementations
### Supervised Learning
- [Adaboost](mlfromscratch/supervised_learning/adaboost.py)
- [Bayesian Regression](mlfromscratch/supervised_learning/bayesian_regression.py)
- [Decision Tree](mlfromscratch/supervised_learning/decision_tree.py)
- [Elastic Net](mlfromscratch/supervised_learning/regression.py)
- [Gradient Boosting](mlfromscratch/supervised_learning/gradient_boosting.py)
- [K Nearest Neighbors](mlfromscratch/supervised_learning/k_nearest_neighbors.py)
- [Lasso Regression](mlfromscratch/supervised_learning/regression.py)
- [Linear Discriminant Analysis](mlfromscratch/supervised_learning/linear_discriminant_analysis.py)
- [Linear Regression](mlfromscratch/supervised_learning/regression.py)
- [Logistic Regression](mlfromscratch/supervised_learning/logistic_regression.py)
- [Multi-class Linear Discriminant Analysis](mlfromscratch/supervised_learning/multi_class_lda.py)
- [Multilayer Perceptron](mlfromscratch/supervised_learning/multilayer_perceptron.py)
- [Naive Bayes](mlfromscratch/supervised_learning/naive_bayes.py)
- [Neuroevolution](mlfromscratch/supervised_learning/neuroevolution.py)
- [Particle Swarm Optimization of Neural Network](mlfromscratch/supervised_learning/particle_swarm_optimization.py)
- [Perceptron](mlfromscratch/supervised_learning/perceptron.py)
- [Polynomial Regression](mlfromscratch/supervised_learning/regression.py)
- [Random Forest](mlfromscratch/supervised_learning/random_forest.py)
- [Ridge Regression](mlfromscratch/supervised_learning/regression.py)
- [Support Vector Machine](mlfromscratch/supervised_learning/support_vector_machine.py)
- [XGBoost](mlfromscratch/supervised_learning/xgboost.py)

### Unsupervised Learning
- [Apriori](mlfromscratch/unsupervised_learning/apriori.py)
- [Autoencoder](mlfromscratch/unsupervised_learning/autoencoder.py)
- [DBSCAN](mlfromscratch/unsupervised_learning/dbscan.py)
- [FP-Growth](mlfromscratch/unsupervised_learning/fp_growth.py)
- [Gaussian Mixture Model](mlfromscratch/unsupervised_learning/gaussian_mixture_model.py)
- [Generative Adversarial Network](mlfromscratch/unsupervised_learning/generative_adversarial_network.py)
- [Genetic Algorithm](mlfromscratch/unsupervised_learning/genetic_algorithm.py)
- [K-Means](mlfromscratch/unsupervised_learning/k_means.py)
- [Partitioning Around Medoids](mlfromscratch/unsupervised_learning/partitioning_around_medoids.py)
- [Principal Component Analysis](mlfromscratch/unsupervised_learning/principal_component_analysis.py)
- [Restricted Boltzmann Machine](mlfromscratch/unsupervised_learning/restricted_boltzmann_machine.py)

### Reinforcement Learning
- [Deep Q-Network](mlfromscratch/reinforcement_learning/deep_q_network.py)

### Deep Learning
  + [Neural Network](mlfromscratch/deep_learning/neural_network.py)
  + [Layers](mlfromscratch/deep_learning/layers.py)
    * Activation Layer
    * Average Pooling Layer
    * Batch Normalization Layer
    * Constant Padding Layer
    * Convolutional Layer
    * Dropout Layer
    * Flatten Layer
    * Fully-Connected (Dense) Layer
    * Fully-Connected RNN Layer
    * Max Pooling Layer
    * Reshape Layer
    * Up Sampling Layer
    * Zero Padding Layer
  + Model Types
    * [Convolutional Neural Network](mlfromscratch/examples/convolutional_neural_network.py)
    * [Multilayer Perceptron](mlfromscratch/examples/multilayer_perceptron.py)
    * [Recurrent Neural Network](mlfromscratch/examples/recurrent_neural_network.py)

## Contact
If there's some implementation you would like to see here or if you're just feeling social,
feel free to [email](mailto:eriklindernoren@gmail.com) me or connect with me on [LinkedIn](https://www.linkedin.com/in/eriklindernoren/).
