# Machine Learning Project
## Two-Spiral Task
In this project, the famous two-spiral task is solved using Support Vector Machines (SVM) and Artificial (feed-forward) Neural Networks (ANN). With ANNs, a multilayer perceptron was trained to correctly classify the (x,y) coordinates of the two-spiral coiling three times around the origin. The original dataset of Lang and Witbrock with 194 training points was first solved. Then a series of variations of the task were generated; starting with a lot of data points and reducing the number of points at each step. The associated classification task was solved and compared to each other. This is repeated using SVMs and the results are compared.

For each classification task, different architectures and parameters were used to optimise the performance. For ANNs, the number of hidden layers/units and the use of momentum were the main variations explored. While for SVMs, it was the C and gamma parameters that were varied.

The generalisation ability of the trained classifiers are tested by evaluating it on a test set of all pixels in a section of the (x,y)-plane. Error curves are used to demonstrate the convergence times. The results are contained in the report.
