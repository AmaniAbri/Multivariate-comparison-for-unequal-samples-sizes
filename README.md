# Multivariate-comparison-for-unequal-samples-sizes

## Describsion

Using Dunnett-Tukey-Kramer (DTK) test is useful to compare samples with differnt variance and different sample sizes. This test is useful to compare observations on a pairwise level. Two vectors must be created: observations and the factor level of each observation. A confidence level box plot is produced for ecach of pairwise comparison. 

## Installtion 

```ruby
install.packages("DTK")

```

## Loading  data
```ruby
setwd("dir")
dat=as.matrix(read.table("filename"))


View(dat)
A <- dat[, 1]
B <-dat[, 2]
C <-dat[, 3]
```
##  Creating factors using ANOVA
```ruby
dat.anova=as.matrix(read.table("filename"))


FAC <-factor(dat.anova[, 3])

```

## Convert dataframe columns from factors to characters
 ```ruby
 
factors <- as.character(FAC)


```

## DTK: A & factors
```ruby
DTK.result<-DTK.test(x=A,f=fators,c,a=0.05)
DTK.result
DTK.plot(DTK.result)

## Boxplot
boxA <- boxplot(A~factors)

```







