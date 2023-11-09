# Project work 1

``` R
install.packages("ggplot2")
library("ggplot2")
head(diamonds)
```

## Exercise 1

``` R
cut_counts = table(diamonds$cut)
cut_percentages = round((cut_counts / sum(cut_counts)) * 100, digits = 2)

cut_percentages
ggplot(diamonds, aes(x = cut, fill = cut)) + geom_bar()
```

Most common cut type is ideal. 40% of cuts are ideal. 
Percentages:

Fair = 2.98,
Good = 9.10,
Very good = 22.40,
Premium = 25.57,
Ideal = 39.95

![Rplot](https://github.com/viluuu/Insights-from-data-DNK-3621420-3004/assets/101949309/64a2c36b-2623-4208-bcf3-3b3eb75fd391)

![Rplot01](https://github.com/viluuu/Insights-from-data-DNK-3621420-3004/assets/101949309/04665c5c-92fc-4dc3-8cfe-26da0e53f479)

