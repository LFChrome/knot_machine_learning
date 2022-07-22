# knot_machine_learning

## **Summer2022 Weekly ToDos:**

#### [Week 7/19/22-7/26/22]
Meeting Summarize: 
1. Went through basic ideas of Principle Component Analysis and Singular-Value Decomposition to reduce dimensionality of data. 
2. Gathered data set and discusessed about this week Todos. 
3. Might need to learn about other modules (e.g. pytorch, tensorflow, keras, jax) in the future. Scikit-learn is the easiest one to use for now. 

Todo List: 
- [x] Download the dataset (download the .csv/.xls file from **Knot info**.
- [x] Create a github repository (use folders to organize codes and informations). 
- [ ] Use Jupyternotebook to import the dataset.
    - Learn about existing modules for importing dataset from .csv/.xls to python coding environment. 
    - Import the dataset as dataframe (which is consisted by arrays and labels; easier for later usage). 
        - This could be done by using pandas module (learn about how to access data in the module. 
    - Might need to find rows with missing values and throw away those rows. 
- [ ] Try some basic examples with linear regressing using the imported dataframe. 
    - e.g.1. See if Jones polynomial can predict signatures for knots. 
        - *NOTICE: If the data is stored as strings, need to first convert the string into numbers and store the numbers (using sage might be more convenient for the conversion).*
        - Arising Problem: How do we/What is the best way to organize these numbers into features for machine learning?
            - Idea1: Extract the coefficient -> New Problem: there might be infinite number of features BUT we have a finite data set, so this idea is applicable.
            - Idea2: Use evaluations (p(1) p(2) p(3) ... p(n) to high enough dimension so correct coefficient could be solved and computed)
    - e.g.2. Predict alternating form using Khovanov homology. 
        - *NOTICE: Similar problem of storing string data as above (sage could handle polynomial rings). Use functions in sage for storing data.*
