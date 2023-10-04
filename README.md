# Finding-MLE-Using-Grid-Search-Method
This repository contains R-code for finding the maximum likelihood estimator for the standard distributions.<br>
Direct Search Method <br> 
Subtopic: Grid Search Method and Using it to Find Maximum Likelihood Estimator <br>

#que1: Find MLE in case of Bernoulli distribution <br>
n = 1000 <br>
p = 0.6<br>
x = rbinom(1,n,p) # Genrating a random sample from Bernoulli(0.6)<br>
p = seq(0,1,0.001) # Creating vector of different values of the parameter<br>
lf = p^sum(x)*(1-p)^(n-sum(x)) #Writing likelihood function for Bernoulli distribution<br>
mle = p[which(lf==max(lf))] #extracting MLE<br>
mle<br>

