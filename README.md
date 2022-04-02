# Assignment-9-Workflows-Part-2
```{r}
library(readr)
desertrate <- read_csv("~/Desktop/PSY 4960/desertrate.csv")
View(desertrate)
```

```{r}
summary(desertrate$dessert)
summary(desertrate$rate)
summary(desertrate$quantity)
```

```{r}
library(ggplot2)
ggplot(desertrate, aes(rate, quantity, color=as.factor(dessert)))+geom_point()+theme_classic()
```
