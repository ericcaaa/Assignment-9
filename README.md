# Assignment-9

```{r}
library(readr)
dessertRate<- read.csv("/Users/ericazheng/Desktop/Dessert.csv")
View(dessertRate)

summary(dessertRate$Dessert)
summary(dessertRate$Rating)
summary(dessertRate$Number)

library(ggplot2)
ggplot(dessertRate, aes(Rating, Number, color=as.factor(Dessert)))+ geom_point() + theme_classic()

```
