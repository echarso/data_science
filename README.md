# data_science
#v2 rational thinkking

# Linear programing
Objective minimize maximize cost 
set constraints 
set variables 
run the solver 

## Multiple Objective Linear Programing 

# Integer programming 

# Goal programing 

# Pareto Line

# what are the axioms so a decission to be rational

1.prospective orientation : decission should be based on the consequences

2.transitivity : if A>B , B>C then A>C

3.invarience : same options should lead to same decession no matter what how the options are phrased

4.indepedent from irrelevant alternativess : 
if i preffer A over  B then i should continue prefer A > B not matter if a 3rd alternative come 

# components of a decission

1. alternatives : what you can choose to do

2. objectives : what is to acheived

3. consequences : what happens if an alternative is choosen and a particular event takes place

4. uncertainities : what is outside of our control comes with events

5. preferences : ranking gof conssequences

### One alternative imply a number of possible consequences each one with a propability

# visualize a decision problem 

## influence diargam 


## decission trees 

4 components:



alternative/ decision nodes

event/propability nodes

consequence / value nodes

lines / edges 

# video  7 system of objectives
http://play2.dsv.su.se/Play/ca5601d7a39a47c3bac8dec8b16f96971d

natural preference

artifitial attribute example and preferential independence

proxy attribute

video 8 and 9 not red 10 value functions not finished


# additive model to work 

## preferential indepedence 
The possible levels of one attribute are affecting always in the same way the total value independent of the possible levels of the other attributes

If i prefer a blue volvo > yellow volvo then i will prefer a blue fiat > yellow fiat


defference indepedence for measurable attributes in additive models

# trade off method 

We need to have individual value functions for the attributes. 

Then we construct indefference statements with pairing artifficial alternatives. 

one pair of artifficial alternatives should differ on the level of all attributes exept on one attribute which should have same value in boths alternatives.

Then we construct the relevant equsations that derive from the indifference statements and by also having in mind that the sum of weights = 1 we solve the problem 


# swing method 

From a variety (n) of attributes we construct the following alternatives

1. where all the attributes have their worst values

2 n alternatives where alla tributes have worst expect 1 out of n that has the best

worst alt takes zero points and we ask experts to assing points to the rest with a scale till 100

then we use the following formula to calculate weights wi = pointi / sum_of_points


