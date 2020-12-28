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
Information gain : In a decission tree we would like to 



