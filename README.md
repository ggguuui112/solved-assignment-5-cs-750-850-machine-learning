Download Link: https://assignmentchef.com/product/solved-assignment-5-cs-750-850-machine-learning
<br>
<h1>Problem 1 [25%]</h1>

It is mentioned in Chapter 7 of ISL that a cubic regression spline with one knot at <em>ξ </em>can be obtained using a basis of the form <em>x</em>, <em>x</em><sup>2</sup>, <em>x</em><sup>3</sup>, [<em>x − ξ</em>]<sup>3</sup><sub>+</sub>, where [<em>x − ξ</em>]<sup>3</sup><sub>+ </sub>= (<em>x − ξ</em>)<sup>3 </sup>if <em>x &gt; ξ </em>and equals 0 otherwise. We will now show that a function of the form

<em>f</em>(<em>x</em>) = <em>β</em><sub>0 </sub>+ <em>β</em><sub>1</sub><em>x </em>+ <em>β</em><sub>2</sub><em>x</em><sup>2 </sup>+ <em>β</em><sub>3</sub><em>x</em><sup>3 </sup>+ <em>β</em><sub>4</sub>[<em>x − ξ</em>]<sub>+</sub><sup>3</sup>

is indeed a cubic regression spline, regardless of the values of <em>β</em><sub>0</sub>,<em>β</em><sub>1</sub>,<em>β</em><sub>2</sub>, <em>β</em><sub>3</sub>,<em>β</em><sub>4</sub>.

<ol>

 <li>Find a cubic polynomial</li>

</ol>

<em>f</em><sub>1</sub>(<em>x</em>) = <em>a</em><sub>1 </sub>+ <em>b</em><sub>1</sub><em>x </em>+ <em>c</em><sub>1</sub><em>x</em><sup>2 </sup>+ <em>d</em><sub>1</sub><em>x</em><sup>3</sup>

such that <em>f</em>(<em>x</em>) = <em>f</em><sub>1</sub>(<em>x</em>) for all <em>x ≤ ξ</em>. Express <em>a</em><sub>1</sub>,<em>b</em><sub>1</sub>,<em>c</em><sub>1</sub>,<em>d</em><sub>1 </sub>in terms of <em>β</em><sub>0</sub>,<em>β</em><sub>1</sub>,<em>β</em><sub>2</sub>,<em>β</em><sub>3</sub>,<em>β</em><sub>4</sub>.

<ol start="2">

 <li>Find a cubic polynomial<em>f</em><sub>2</sub>(<em>x</em>) = <em>a</em><sub>2 </sub>+ <em>b</em><sub>2</sub><em>x </em>+ <em>c</em><sub>2</sub><em>x</em><sup>2 </sup>+ <em>d</em><sub>2</sub><em>x</em><sup>3</sup></li>

</ol>

such that <em>f</em>(<em>x</em>) = <em>f</em><sub>2</sub>(<em>x</em>) for all <em>x &gt; ξ</em>. Express <em>a</em><sub>2</sub>,<em>b</em><sub>2</sub>,<em>c</em><sub>2</sub>,<em>d</em><sub>2 </sub>in terms of <em>β</em><sub>0</sub>,<em>β</em><sub>1</sub>,<em>β</em><sub>2</sub>,<em>β</em><sub>3</sub>,<em>β</em><sub>4</sub>. We have now established that <em>f</em>(<em>x</em>) is a piecewise polynomial.

<ol start="3">

 <li>Show that <em>f</em><sub>1</sub>(<em>ξ</em>) = <em>f</em><sub>2</sub>(<em>ξ</em>). That is, <em>f</em>(<em>x</em>) is continuous at <em>ξ</em>.</li>

</ol>

<h1>Problem 2 [25%]</h1>

Use linear, cubic, and natural regression splines investigated Chapter 7 of ISL to the Auto data set. Is there evidence for non-linear relationships in this data set? Create some informative plots to justify your answer.

<h1>Problem 3 [25%]</h1>

You will now derive the Bayesian connection to the lasso as discussed in Section 6.2.2. of ISL.

<ol>

 <li>Suppose that <em>y<sub>i </sub></em>= <em>β</em><sub>0 </sub>+ <sup>P<em>p</em></sup><em><sub>j</sub></em><sub>=1 </sub><em>x<sub>ij</sub>β<sub>j </sub></em>+ <em><sub>i </sub></em>where <sub>1</sub><em>,…,<sub>n </sub></em>are independent and identically distributed from a normal distribution <em>N</em>(0<em>,</em>1). Write out the likelihood for the data as a function of values <em>β</em>.</li>

 <li>Assume that the prior for <em>β </em>: <em>β</em><sub>1</sub><em>,…,β<sub>p </sub></em>is that they are independent and identically distributed according to a <em>Laplace </em>distribution with mean zero and variance <em>c</em>. Write out the posterior for <em>β </em>in this setting using Bayes theorem.</li>

 <li>Argue that the lasso estimate is the value of <em>β </em>with maximal probability under this posterior distribution. Compute log of the probability in order to make this point. <em>Hint</em>: The denominator (= the probability of data) can be ignored in computing the maximum probability.</li>

 <li>Suppose that <sub>1</sub><em>,…,<sub>n </sub></em>are independent and identically distributed according to the Laplace distribution.</li>

</ol>

What are the maximum likelihood/MAP estimates of <em>β<sub>i </sub></em>under this assumption? <em>Hint</em>: See <a href="https://en.wikipedia.org/wiki/Least_absolute_deviations">https: </a><a href="https://en.wikipedia.org/wiki/Least_absolute_deviations">//en.wikipedia.org/wiki/Least_absolute_deviations</a>

1

<h1>Problem 4 [25%]</h1>

<em>Based on a true story, according to</em>: The Drunkard’s Walk: How Randomness Rules Our Lives, Leonard Mlodinow

Suppose that you applied for a life insurance and underwent a physical exam. The bad news is that your application was rejected because you tested positive for HIV. The test’s <em>sensitivity </em>is 99<em>.</em>7% and <em>specificity </em>is 98<em>.</em>5% <a href="https://en.wikipedia.org/wiki/Diagnosis_of_HIV/AIDS#Accuracy_of_HIV_testing">[https://en.wikipedia.org/wiki/Diagnosis_of_HIV/AIDS#Accuracy_of_HIV_testing]</a>. However, after studying the CDC website, you find that in your ethnic group (age, gender, race, …) only one in 10,000 people is infected. What is the probability that you actually have HIV?

2