# week 7 introduction to machine learning

## introduciton to machine learning
https://youtu.be/Bxd26C9aDis

SciKit learn - machine learning library, introduction into getting understanding of machine learning options. Will be able to create simple machine learning algorthyms
Aim to explain what machien leanring is and 3 applications
Focuses on computer systems that can learn from data, often called models. Can perform specific task by analyising lto sfo exmaples for a particular problem. Can learn to recognise image of a cat by being shown lots of images of cats.
Means it can learn a specific task on its own.
Programmed to learn on its own.

Model learns on its own to determine what it is e.g. if data contains a cat from what is analysed.
Amount and quality of data available are important thing in how accurate model wil be.
Can be used ot discover hiddne trends and patterns in data.
Can then create useful insights from the data.


Many examples of machine learning applications

Credit card fraud detection 
- every time used, current purchase analyised against prior purchase to see if legitimate transaction or potentially fraudulent one. 
- e.g. big ticket item in one dont usually buy or from another country, may be denied or may get call from credit card company.

Hand written cheque machine learnt process. 
- Machien leanring to go through patterns.
- this reads hand written numbers to identify the information
- more difficult to detmerien due to diference sin hadnwriting compared to typed responses
- machine learning patterns helpful to detmerine differences

Recommendations on websites 
- after buying item often list of related items, customer who bought this item also bought these. Related items associated using machine learning model. Common application used in sales and marketing.

Machine learning terms
- Data mining 
-- linking and use databases to analyse information
- Predictive analytics 
-- predicting purchases and information, usually used in buisness to describe sales forcasting adn predicitng purchaisng behaviour of a customer

- Big data 
-- data sciecne extracting meaning for collecting, storing and managing as well as machine learning insights from big data


## categories of machine learning
https://youtu.be/MUWoy1GpkFo

classification
regresssion
cluster analysis

supervised learnign

-classification

goal to predict gategory

e.g. predcitign weather as sunny, windy rainy, cloudy
input data, temp, pressure, wind pressure
target differetm weather catgetory


e.g. classify tumour benign or maligannt
would be binary as only two options

e.g. identify handwritten digits
one of ten categroys 0-9

- regresiion

goal predict numeric value

e.g. predict price of a stock
this would be for actual stock

if it was looking if stock rise or fall that would be classification instead as a category


e.g.
amount of rain for a region

-Cluster analysis

goal to organise similar items into groups

customer segmentation is an example
putting customers into differnet groups
e.g. sensiors, adults and teenagers
as they have different purchainsg behaviours

may lead to targetted advertisments for each group



- association analysis

goal find rules to capture assocaitison between items

rules to detmerien when items or evnst occur together
e.g. market basket analysis
used to detemrein customer purchase bhevaiour

e.g. can reveal banking custmoers who have purchaisng accounts may be interestd in antoher type
this can be used for cross selling 

e.g. recommendations of similar items based on purcahsing or browsing history of customers
finding items often purchased together to offer these to drive sales of them all

e.g. idnetinfy of web pages often open together
give offers on associated web pages


- supervised vs unsueprvised learning

supervised approaches
-- target provided - what model is predicting
-- labeleld data
-- classification and regerssion are supervised


unsupervised approaches
-- target is unknown or unavailable
-- unlabled data
-- cluster analysis and association analysis are unsupervised



## terminology related to machine learning
https://youtu.be/4-BXXzMJuk8

feature and how ti relate to a sample
name altnerive terms for af eature

terms to describe data

samples
- instances or example of entity in your data
- typically row in dataset
- record
- observation
- instance

variables
- values associated with each sample
- e.g. date, min temp, max temp, rainfall
- sometimes referred to as features of the sample
- dimension
- attribute
- field
- column


each variable has a data type associated with it

most common
- numerica
- categoryical

other types
- string
- date

numerical varlaibes
- values are numbers
- can be sorted in order in some way
- can take on integer or could be continuosu
- can be negative only postiive, or both

categorical variables
- colour of an item
- values could be red, silver, blue, black
- non numeric value that describes an entity



## scikit learning, machien learning in python
https://youtu.be/y5d23KWvThA

scikit learning library for machine learning
navigate way to right tool in scikit learn
search for tutoris that provide prbem specific emapdes using library functions

scikit-learn open source library for machine lernign in python
built onotp of numpy, scipy, matplotlib
improved continuously

end ot end machine learning

entire process canb e dodne


- prepresosing tools

utiliy functions for transfomring raw feature vecutros

provides api for scaling of feature
normalsiation
missign value handling

has functions built in for clustering and types of infmraiotn

documentation includes tutorials on website as well

sklearn.cluster 
0 gives alogorhyitms for grouping of unlabeleld data

has special features for dimensionatliy reduction - helpful for many factors

provides full set of tools and can use in python with other data science tools




## Notebook: Introduction to Machine Learning
Bookmark this page
Please download the notebooks for this week so you can follow along with us during the videos and play with the code yourself.

# classification
## classification
https://youtu.be/0T6aYa2U8ug

task is to predcit category from input variables by making a model that can predict accurately
labelled data so is a supervised task
classification can be 
-binary just two options or
- multi class - more than two types of values, sometiesm called multinominal

model has to predcit category considering input variables


## building and applying a classificaiotn model
https://youtu.be/b7LQ6yYw4pA

- building classifciation model
- applying a classifciation model

machine learnign model is a mathematical model with parameters that map inputt to output
- model adjusts parametres to refine inputa and output parameters

traiing model and building using the right formualr and ifnormaiton from input variables
classification decisions based on boundaries between decisions

- decision boundaries
use datat to adjsut mdoels parametsr in order to fomr decision boudnires to serpate dcision calsses

two phaes
1. traingn hpase
- adjust model parameter
- use training data

2. testing phase
- learned model applied
- used with new data


at end of trainign phase get traiend model
testing phase use traiend model is applied to test data to get test results
can then evaluate model based on how it performs on the test data

commonly used algorhyms for building classification model
task: predict categroy from input varilsbes
goal: match model outputs to targets (desired outputs)

learning algorithm used to adjut models paremtsrs

-kNN
- decision tree
- naive baytes

kNN
k nearest neighbours
this technique relies on samples are similar by looking at cloest neighbours

decision tree
- classifciaiton model uses three like structure
e.g.
warm blooded
- live birth or non mammal


naive baytes
- probablsitic approahc to classificaiotn

bayes' theorem
compares the probabitly of an event in the presce of another event

probaitlyi of having a fire if the weather is hot


## decision trees
https://youtu.be/ksQXxH8W50I

decision tree overview

idea: split data into "pure" regions
- each subset contains as many subsets of same class
- boundaries seperating these regions are called decision boundaries

decision tree is heirachy strucutre with nodes and directional edges
root node - at top
internal node - within root and leaf nodes
leaf nodes - at bottom

at each node conditino determiens which branch to go to 
when final leaf node is reached detemriens answer to classification decision
depth of a decision tree is lgonest path from root node to leaf node
size of tree is number of ndoes ina  tree

example decsion tree

warm blooded 
---- live birth
---- vertebrate
= mammale

if none of these then not mammal

construcitn decision tree

starts at root node and adding as subsets are created

- start with all samples at a node
- partition sapes based on input to create purest subsets
- subsets should be homogenous - or as pures as possible
- repeat to parttion data into succesisvley prue subsets

this is refered to as a tree induction algorythm

greedy approach
at each split algothrym consdiers best way to split that algothrym
solves subset at a time so cant solve at the same time

not feaslb to determine best stree given dataset so has to be best way to split tree at each node then combing deisiont o get final informaiotn

more homogenous = more pure

impurity measure
- to compare different wayst o split data in a node
- works better to measure purity
- how mixed resultign subsets are 
- aimginf or split that minimises impurity measure

- gini index - common measure, the lower gini index the higher the split
- entropy
- infomraiton gain
- misclassificaiton rate


What variable tosplit on?

- splits on all variables are tested

when to stop splitting a node?

- all or(e.g. 90 )% of samples have same class label
- number of samples in nodes reaches minimum
- change in impurity measures is smaller than threashold
- max tree depth is reached
- others

Tree induciton example

split loan applicants to those liekly ot pay and those not liekly to pay based on incmoen and amountof debt they have
consdier input space, consider decision boundry where incomine is t1, so to right mostly repayments but to left mostly non payments
----- split at income > t1 passed to next node
next how to split region when debt =t2

---- debt >t2
splits to show those that are lekly to repay and another to pass to next node

3rd split and final loks at incmine again bounday = t3
splits into two pure subsets
---- incomien > t3

final decision boundaryes from decison boundaries
they partition data set

decision boundaires are parrael to axies
rectilinear = parallel to axes

variants that consider more than one variable but require more computational expensive



decsiion tree for classficaiont

- resultign tree is often simple and easy to interpret
- induction is computationally inexpensive
- greedy approach does not guarentee best soltion
- rectilinear decision boundaries

decision tree created by continosuyl splitting data
resulting tree often easy to interpret

end of 5/5/2020

## live code, decision trees
https://youtu.be/TeAbMoLdmvk

start 6/5/2020

data set from weather station from sep 2014 to sep 2017
using classficiaont of weather data using decsion trees




# clustering
## clustering
https://youtu.be/kmVBDGMgeWI

## k-means clustering
https://youtu.be/uWm5X3dIu5k

## live code, clustering
https://youtu.be/vTMILyEhbn0


## regression analysis
https://youtu.be/jSRh1Het59k

## linear regression
https://youtu.be/0U-0PTDV64g

## live code, linear regression
https://youtu.be/PjbTG5BNzL0

## Notebook: Coding Practice
Bookmark this page
It's important to get practice with the programming concepts of the week.  If you haven't already done so, please download the notebooks for this week and work through the examples.

If you want to practice and test your knowledge by developing other notebooks, you can access these by signing up for the Verified Certificate program -- for those looking to more robustly document their knowledge and skills.  This can also put you on the path to earning a MicroMasters in Data Science, if that would be helpful to you!


