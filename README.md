# Scientific Computing 2024
Scientific Computing is an extra course I teach at the [JetBrains](http://jetbrains.com) and [Constructor
University](https://constructor.university) (Bremen) [Software, Data and
Technology](https://lp.jetbrains.com/software-data-and-technology-constructor-university/) bachelor probgram in fall
semester of 2024-25 academic year. This repository will contain materials of the
course (lecture notes, notebooks), available under MIT license.

The course is aimed at bridging the gap between pure mathematical
courses and machine learning. We will discuss various concepts, some of
which are already known to the students and some are new, in applied and
computational context. We will also learn how to use various programming
tools to interact with mathematical objects and visualize them.

## Prerequisites

The students are expected to know Calculus (of one and many variables),
Linear Algebra and be able to program in Python.

## Topics

One topic is approximately one week (maybe more), 2 lessons, 75 minutes
each lesson.

### Overview of scientific Python ecosystem

Jupyter notebooks: pro and contra, best practices. Package managers:
`pip` and `conda`. Virtual environments. Reproducibility issues. Basic
numerical and data science packages: `numpy`, `scipy`, `matplotlib`,
`pandas`. Introduction to `numpy`: `array` vs. `list`, why do we need
arrays, idea of vectorized calculations. Plotting of basic graphs with
`matplotlib.pyplot`. Interactive widgets, `%matplotlib widget`.
Animations with `IPython.display`.

### Numerics in Python

#### Numerical types

Numerical types in Python. `int` vs. `np.int64`. Floating point
arithmetic. `NaN` and `Inf`. `0.1 + 0.2 != 0.3`. Numerical precision.
Machine epsilon. Numerical (in)stability. Example: numerical derivative.
Calculation in logarithms, `logsumexp`, example: `softmax`.

#### More on `numpy`

Shape, reshaping data. Advanced indexing, `np.where`. Broadcasting
rules. Matrix multiplication. `np.linalg`. How to get rid of `for` loops
with `numpy` magic. Memory cost of vectorization. Processing by batch.

### `pandas`

`pd.Series` and `pd.DataFrame`. Constructing dataframes. Indexing.
Queries. Grouping and aggregating. Concatenating and merging dataframes.
Melting and pivoting.

### Visualization I: `matplotlib` and low-level stuff

Introduction to plotting in Python. Example: gradient descent.

### Visualization II: `seaborn`, `plotly` and data

How to choose the best visualization method: case study.

### Linear algebra I

Linear systems. Over- and underdetermined systems. Pseudoinverse,
pseudosolution, normal pseudosolution. Geometrical interpretation.
Matrix factorizations. Application of factorizations to solution of a
linear system.

### Optimization

Theory recap: optimization of function of one variable, conditional
optimization, Lagrange multipliers. Numeric optimization of function of
several variables. Gradient descent. Example: gradient descent near a
minimum with ill-conditioned Hessian. Newton's method. Optimization of
matrix-vector functions. Optimization out of the box: `scipy.optim`.

### Probability I

Random variables. Discrete and continuous distributions. Cumulative
distribution function. Expected value, variance. Generating (pseudo)
random numbers. Seed. `np.random` and `scipy.stats`. Probability density
function and histogram. Rejection sampling. Transformation of random
variables. Entropy. KL-divergence.

### Probability II

Independent and non-independent random variables. Joint distribution
(continuous + continuous, continuous + discrete, discrete + discrete).
Covariance and correlation. Variance-covariance matrix and correlation
matrix. Conditional distribution, conditional expectation. Central limit
theorem. Monte-Carlo integration. Mutual information.

### Linear algebra II

More on matrix factorization. Symmetric matrices and quadratic forms.
Positive definite matrices, their properties. SVD decomposition,
low-rank approximations. Example: covariance matrix as a quadratic form.

### Statistics I

Random variables and samples. Statistical estimates. Consistency,
unbiasedness. Likelihood. MLE.

### Statistics II

Statistical hypothesis testing. Type I and type II errors. Student's
t-test. Permutation test.

### Bonus: elements of Bayesian statistics

### Bonus: analysis of graph data

## Assessment

Every week, there will be a homework. Each homework consists of problems
of various difficulty. It is indicated how many points the complete and
correct solution of each problem earns. Some of the problems are marked
as bonus. The final grade (on a scale from 0 to 10) is calculated as a
sum of all earned points (including points for bonus problems)
multiplied by 10 and divided by the sum of all points of non-bonus
problems.

For each homework assignment, there will be specified a due date and a
hard deadline. If the assignment is returned after the due date, but
before the hard deadline, its score is multiplied by $e^{-t/86400}$,
where $t$ is number of seconds passed since the due date. If the
assignment is returned after the hard deadline, it is scored as 0.
