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
Factors <-dat[, 3]
```
##  Creating factors using ANOVA
```ruby
dat.anova=as.matrix(read.table("filename"))


FAC <-factor(dat.anova[, 3])
BB <-factor(dat.anova[, 2])
AA <- factor(dat.anova[, 1])

```

## Convert dataframe columns from factors to characters
 ```ruby
 
FF_Ch <- as.character(FAC)
BB_ch <- as.character(BB)
AA_ch <- as.character(AA)

```





