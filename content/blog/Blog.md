---
title: Basic R Studio and Python Interactions
author: Kylie Wakefield
date: '2020-05-12'
linktitle: Cool Python Things
highlight: yes
---

Python and R can interact together by utilizing the reticulate package. Through this package, the {r} and {python} code chunks will talk to one another. 

One cool thing about python is it's ability to create strings. The strings can be a collection of words or phrases. Here are some of my favorite foods...

```{python}
#python code chunk

'ice cream, rasberries, breakfast tacos, and queso'
```
##Output: 'ice cream, rasberries, breakfast tacos, and queso'

They can also be saved as an object, like R!

```{python}
#python code chunk

favoritefoods = "ice cream, rasberries, breakfast tacos, and queso "
favoritefoods
```
##Output: 'ice cream, rasberries, breakfast tacos, and queso '

When r and python interact together, the two objects can be shown by using the print() function. The print() function also gives a cleaner output of the strings. (r."object") allows the python code to output the r object allow with the string in the python code. Pretty cool! 

```{r}
#r code chunk

food<-"my favorite foods are"
```

```{python}
#python code chunk

print(r.food,favoritefoods)
```
##Output: my favorite foods are ice cream, rasberries, breakfast tacos, and queso 

If I wanted to convert all of my favorite foods into upper case letters, then I would  use the str.upper() function. This is really emphasizing my favorite foods. YUM!!!

```{python}
#python code chunk

uppercase = str.upper(favoritefoods)
uppercase
print(r.food, uppercase)
```
##Output1: 'ICE CREAM, RASBERRIES, BREAKFAST TACOS, AND QUESO '
##Output2: my favorite foods are ICE CREAM, RASBERRIES, BREAKFAST TACOS, AND QUESO 

I hope that through my blog you learned a little about python and r studio, as well as my favorite foods. Maybe this while inspire you to indulge in your favorites... :)