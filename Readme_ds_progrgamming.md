# Theory 

# exploratory analysis

1.  normalization z normalization 


    from ever point remove averageg the mean and then devide with variance 
    
    why ? we set the data in a normal sscale and now every data point is treated equally , 
    
    since in every  feature value is represeanted in a correlation the rest relavant feature values. 
    
2. binding 

   real value data are separated rgouped in buckets it helps analysis
   
3. curse of dimentionality 

    high dimentional data and a lot of noise . 
    
    the importance of PCA principal component analysis 
    
    step 1 z- normalization, 
    step 2 find covariance matrix , which describes simularities of features 
    step 3 find the egenvalues for that matrix , select the top ones that describes the most of the dataset
    
    finds the coovaration matrix , and the basic dianysma so data can be represented by this minimal dianissma 
    
# Clustering data unsupervised

## k-means - each datapoint brings its gravity

we need to give as input the possible centers 
#### algorithms randomly selects center values 
calculates euclidian disctance from centers for the iserted data point 

assing the data point to nearest center 

recalculate the center based on means of the data points that belong to center 

adjust centers and re runs 

## k-medodis 

we need to give as input the possible centers 
#### we select datapoints as centers at initialization 

can use any distance measure for assing centers 

recalculate centers and adjust only if it is benefitial 

 
# Classification data , supervised

## Decission trees and random forest 

In decission trees we have nodes and leafs. In every node we run a test in one of our features that seperates / splits our dataset in the correspoing 2 leafs.

Aim is to end up in nodes that cannot be separated/splitted anymore in respect to our classification goal.  For acheiving the above we have 3 basic concepts to. understand . Entropy , information gain and pure. 

We call a set of datapoints / inpputs that is pure if the belong to the same classification unit/set.
For example if my. target is to classify cars vs icecreams .  Then the following datapoints set ( volvo, subaru, vanilla , chocalate) is not pure.
On the contrary this dataset is pure ( volvo, subaru) and. this one also (vanilla , chocalate)

Entropy describes  the level of how not pure a dataset is. Or how much different datapoints we have in a dataset
Information gain : In a decission tree we would like when performing a spliting in a node to end up in a more pure node, in other words in every split we would like to reduce entropy. This reducing of entropy we can describe oor quantify  it as information gain and the algoritgm of decission trees always splits the trees with the test in a value that gives the higher information gain . 

Problem in decission trees.

Which feature we are going to use for starting splitting our dataset? we are going end up with different decission trees when we decide different features for our initials nodes. 

In addition decission trees are subject of overfitting. They learn our dataset too well almosst copying it, so when they are exposed to different data sets that they belong to same family they behave or score bad, because the are unable to generalize well. For example if we allow our decisssion tree to generate alot leafs. and nodes , or in other wordss to have high depth , then they may start classifying inputs based on their exact numeric values we had in our training  datasset.

That is why we have random forests. is a collection of decission trees that are trained in random samples of the dataset . They start with different feature in the node and we don't let them going to high depth . When we classify an entry with random forest the classification decission iss based on the majority vote of the decission trees that consist our random forest. 

This kind of decission can be described as propability of 3 out 10 trees in the forest classify a dataentry as of class A then we can claim that this dataentry has 30% probability to belong to class A and so on . 








