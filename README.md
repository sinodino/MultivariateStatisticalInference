# Multivariate Statistical Inference
Course projects of MSI

Homework 1
Q1. [R] Write a function, named ‘MD’, to calculate Mahalanobis Distance.
Q2. [R] A public opinion poll surveyed a sample of 1000 voters randomly. Respondents were classified by gender (male or female) and by voting preference (Republican, Democrat, or Independent). Results are shown in the contingency table below. Use both visualization and statistical test to tell me something you learn from the data.
Q3. [R] The dataset datahw1.txt contains three variables, without knowing what kind of variables they are, use exploratory data analysis and visualization, including but not limited to summary statistics (means and variances), scatter plot matrix (hint: scatterplotmatrix() or pairs()), report what you find and identify potential outliers.
Q4. [R] Use R dataset ‘UCBAdmissions’ to answer the following questions, you can begin with ?UCBAdmissions & head(UCBAdmissions) to see what kinds of variables the dataset have.
(1) Is there any dependency between gender and admission?
(2) Where (which department) do people apply, any difference between female and male? Is the difference significant?
(3) How selective are all the departments? Is there any department that is more competitive, which department(s) seems hard to get admissions in, which
is/are easier?
(4) Together with your answers to (2) & (3), what else do you find?
(5) Is there any gender bias within the departments, i.e., any department favors one gender over the other?
(6) Anything else? (Bonus)

Homework 2
Q3. [R] Principal Component Analysis on pendigit data from UC Irvine Machine Learning Repository at http://archive.ics.uci.edu/ml/datasets/Pen- Based+Recognition+of+Handwritten+Digits. 
I have already downloaded the dataset for you and save it as a .txt file. The dataset contains 3498 rows observations of 17 columns. The column 1 – 16 are variables of our interest, the last column of the data contains number 0 – 9, represents that the observation is a writing of a digit 0 – 9, e.g. if the column number is 3, it means it is a writing of a digit 3. You can think of this variable like a class variable. You can get better understanding after reading the dataset description. And the columns 1-16 are equal spaced locations of a pen at 8 timepoints, and are arranged as x1, y1,x2, y2,...,x7, y7,x8, y8 , and any pair (xi , yi ) is the location of a pen at timepoint i.
Now use the dataset to answer the following questions:
(1) For different class (last column of the dataset), visualize the first observation for
each class, using line instead of points, what do you see?
(2) Now use the subsetting you learnt in the first R practical section to create a sub-
dataset, name it pendigit3, which only contains class 3, or digit 3 (hint: the last column = 3), perform PCA for this dataset and show the principal components and their associated variances, (hint: you may need scatterplot matrix and scree plot, but if you have better choices, please do).
(3) Based on your plots, do the data look like they are from a Multivariate Normal Distribution? And give me some justification over how many components you would like to keep.
(4) Look at the first 4 principal components one by one, can you explain the feature extrated from the orignal data, and captured by each of these 4 principal component? The feature is also called the modes of variation.
(5) Now use the subsetting you learnt in the first R practical section again to create another subset, name it pendigit38, which contains class 3 and 8. Perform PCA on the new dataset pendigit38, now report what you find from the analysis with plots. (hint: you may still need scatterplot matrix) And since now you have two classes in your dataset, and from Question (1), you know that the plot gives you the digit, do you see a good separation of observations correponding to the two classes?

Homework 3
Q1. [R] [Textbook IAMA Ex. 3.1] Construct the scatterplot of the heptathlon data showing the contours of the estimated bivariate density function on each panel. Is this graphic more useful than the unenhanced scatterplot matrix?
Q2. [R] [Textbook IAMA Ex. 3.2] Construct a diagram that shows the SO2 variable in the air pollution data plotted against each of the six explanatory variables, and in each of the scatterplots show the fitted linear regression and a fitted locally weighted regression. Does this diagram help in deciding on the most appropriate model for determining the variables most predictive of sulphur dioxide levels?
Q3. [R] Load the zehnkampf.dat. The data is the result of the decathlon at the Olympic Games in Atlanta in 1996. You will see that there are 11 variables in total.
(1) Do PCA on the data using both covariance matrix and correlation matrix, visualize your results using available tools you learnt to compare the results of these two, and explain which you think is more advisable.
(2) From the PCA results (the one your chosen from (1)), explain your conclusion about this dataset, here I provide a set of questions to guide you but do go beyond what I am asking, you may observe more interesting results or patterns.
a. Every athelete wants to get the highest total number of points (punkte), which discipline seems crucial or highly related to the total number of points? This may tell atheletes that in order to get to the final 3, they probably need to lead on this discipline.
b. From you visualization, which discipline(s) seem poorly displayed, and which one(s) seem very clear, and what do you think is the reason?
c. Identify disciplines (two or three) that seem like a bundle that atheletes either do well on both (or all) or do poor on both (or all).
d. Identify disciplines (two or three) that seem like a challenge that atheletes hardly do well on both (or all) at the same time.
e. Identify disciplines (two or three) that seem like a challenge for us that we cannot really predict an athelete will do well on one from his/her performance on the other(s).
(3) Identify the average athelete using R function (identify()).
Q4. [R] [Textbook IAMA Ex. 4.1] Consider 51 objects O1, ..., O51 assumed to be arranged along a straight line with the jth object being located at a point with coordinate j. Define the similarity sij between object i and object j as below:
If i=j, sij=9;
If 1<=|i-j|<=3,sij=8;
If 4<=|i-j|<=6,sij=7;
...
If 22<=|i-j|<=24,sij=1;
If 25<=|i-j|,sij=0;

Convert the similarities into dissimilarities by sqrt(sii+sjj-2sij)
and then apply classical multidimensional scaling to the resulting dissimilarity matrix. Explain the shape of the derived two-dimensional solution.
