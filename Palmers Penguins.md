---
title: "Palmers Penguins"
author: "Jen"
date: "2023-09-25"
output: github_document
---

# Palmers Penguins: Body Mass vs. Flipper Length

```{r ggplot for penguin data}
install.packages("vitae")
library(ggplot2)
library(palmerpenguins)
data(penguins)
head(penguins, 8)
```

## Penguin Visualization for Body Mass vs. Flipper Length
This visualization shows that the Gentoo species is the largest penguin of the three based on an increase of flipper length to body mass relationship.
```{r ggplot for penguin data visualization}
ggplot(data= penguins)+
  geom_point(mapping=aes(x=flipper_length_mm, y=body_mass_g, color=species))+
  geom_smooth(aes(flipper_length_mm, body_mass_g))+
  labs(title= "Palmer Penguins: Body Mass vs. Flipper Length")
```

[PalmersPenguins_Rplot.pdf](https://github.com/datash0ck/R-Projects/files/14272146/PalmersPenguins_Rplot.pdf)

