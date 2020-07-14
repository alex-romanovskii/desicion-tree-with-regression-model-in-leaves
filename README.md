# desicion-tree-with-regression-model-in-leaves

**If you have trouble with watching ipynb online, click [Here](https://htmlpreview.github.io/?https://github.com/alex-romanovskii/desicion-tree-with-regression-model-in-leaves/blob/master/project.html) to see code with describtion**  

The goal of the project is to create a decision tree with a regression model in each leaves

The algorithm of the implemented decision tree enumerates all possible options for splitting the dataframe. 
- If it is a numeric column, then dataframe has been split according to the following conditions:
np.linspace (values_min, values_max, num = 10)
in this case, will be binary spliting

- If categorical column, then the OneHot Encoder is applied and the number of partitions is equal to the number of unique values in column

After each partition, a regression model is considered for each received dataframe and the partition is selected in which a weighted MSE gives the best result.

You can see project.ipynb to see implementation algorithm and to see comparison results with Regression Tree 
