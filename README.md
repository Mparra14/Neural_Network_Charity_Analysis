# Neural_Network_Charity_Analysis
## Overview of the analysis: 
In this project we worked with Alphabet Soup, a nonprofit organization that helps raise donations for foundations. We were tasked with finding which foundations would have a higher probability of receiving funds from Alphabet Soup. We were given csv file containing organizations that had successfully received funding by Alphabet Soup. To create a future model that would predict which organization would be eligible for funding, we had to use a new tool called Tensorflow and a new concept called neural network. With neural networking, we must pre-process the data given and find which column of information has the most significant amount of data, once it’s been pre-processed, we must use the columns with significant values and start binning by categories. The data set is then split into test trains and scaled. The model then must be tested and trained and fitted to find the accuracy. 



## Results:

### Data Preprocessing

What variable(s) are considered the target(s) for your model?
* The variable that is the target is the is successful column, since we are trying to find which organizations were funded by Alphabet Soup

What variable(s) are considered to be the features for your model?
* The variables that are the features would be the columns such as application type and classification type.

What variable(s) are neither targets nor features, and should be removed from the input data?
* The variables that were removed were the EIN, Status, and Special considerations. These had the leas significant of values that were not needed. 

### Compiling, Training, and Evaluating the Model

How many neurons, layers, and activation functions did you select for your neural network model, and why?
* Knowing that X-train length is 395 for this model, we had to use more than two layers. As a rule of thumb, the neurons should either be three to two times as much as the length. Having more layers and neurons will have the date be fit faster, than having just one neuron and one layer. This can be seen in the picture below.

![neural_layers]()

Were you able to achieve the target model performance?
* Yes, the target model was achieved with a 78% of accuracy. 

![accuracy_model](https://github.com/Mparra14/Neural_Network_Charity_Analysis/blob/main/model_accuracy.png)

What steps did you take to try and increase model performance?
* One column that I decided to keep was NAME, it had a significant amount of data that would create a better model, also it helps knowing which organizations had successful funding. I dropped the two columns that had the lowest value count which was status and special considerations. When it came to binning the names column it was done just like the application and classification column. 


## Summary: 

The model designed ended with a 78% accuracy, which means the target was achieved, which was much higher than the original model which we got 72% accuracy. One way to keep optimizing the model is by either dropping more insignificant columns such as the organization column it has low value counts, and you can also bin the asking amount column, it has a significant number of categories. A different model that could've been chosen would be random forest classifier this method is able to handle big data as well as attribute to high accuracy levels as well as high performance levels due to each tree.

