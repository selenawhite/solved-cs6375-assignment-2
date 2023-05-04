Download Link: https://assignmentchef.com/product/solved-cs6375-assignment-2
<br>
<strong>Problem:</strong> Implement a <strong>fixed-depth decision tree algorithm</strong>, that is, the input to the ID3 algorithm will include the training data and <strong>maximum depth</strong> of the tree to be learned. The code skeleton as well as data sets for this assignment can be found on e-Learning.

<strong>Data Sets:</strong> The MONK’s Problems were the basis of a first international comparison of learning algorithms [1]. The training and test files for the three problems are named monks-X.train and monks-X.test. There are six attributes/features (columns 2–7), and binary class labels (column 1). See monks.names for more details.

Visualization: The code skeleton provided contains a function render_dot_file(), which can be used to generate .png images of the trees learned by both scikit-learn and your code. See the documentation for render_dot_file() for additional details on usage.




<ol>

 <li>(Autograder Score, 20 points) Your code will be auto-graded and cross-checked with other submissions. The auto-grader will evaluate your code on several different data sets to perform a sanity check. In order to ensure that your code passes the auto-grader, ensure that you <strong>do not modify the function headers</strong>. In addition, do not hard code any values (such as y = 0 and 1) and make your code as general as possible.</li>

</ol>




<ol>

 <li>(Learning Curves, ) For depth = 1, …, 10, learn decision trees and compute the average training and test errors on each of the three MONK’s problems. Make three plots, one for each of the MONK’s problem sets, plotting training and testing error curves together for each problem, with tree depth on the x-axis and error on the y-axis.</li>

</ol>




<ol start="5">

 <li>(Weak Learners, ) For monks-1, report the visualized learned decision tree and the confusion matrix on the test set for depth = 1, 3, 5. You may use scikit-learns’s confusion matrix() function [2].</li>

</ol>




Figure 1: Confusion matrix for binary Classification Problem




<ol>

 <li>(scikit-learn, 20        points)             For       monks-1,         use scikit-learn’s</li>

</ol>

DecisionTreeClassifier [3] to learn a decision tree using criterion=’entropy’ for depth = 1, 3, 5. You may use scikit-learn’s confusion matrix() function [2].




<ol>

 <li>(Other Data Sets, 20 points) Repeat steps (c) and (d) with your “own” data set and report the confusion matrices. You can use other data sets in the UCI repository. If you encounter continuous features, consider a simple discretization strategy to pre-process them into binary features using the mean. For example, a continuous feature x can be discretized using its mean µ as</li>

</ol>




Write a report with the solutions to the questions above, showing the plots, confusion matrices and a brief discussion (4–5 lines) comparing your implementation to that of scikit-learn, which is a widely-used, publicly-available, open-source implementation.

[1]https://archive.ics.uci.edu/ml/datasets/MONK’s+Problems

[2]https://scikit-learn.org/stable/modules/generated/sklearn.metrics.confusion_matrix.html

[3]http://scikit-learn.org/stable/modules/generated/sklearn.tree.DecisionTreeClassifier.html