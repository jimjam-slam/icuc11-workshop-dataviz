# Welcome to the datavis workshop!

You've opened the workshop cloud environment!

There are two fils we're going to use today:

[`slides.qmd`](/slides.qmd) is the content of the slides that I'll present. If you'd like to follow along with them, open the file and click the "Render" button up the top right.

[`exercises.qmd`](/exercises.qmd) contains the code for the plots we'll play with today. When you open the file, you'll see "chunks" of code that look like this (with different colours!):

```{r}
#| label: sample-plot

ggplot(mtcars) + 
  aes(mpg, hp) +
  geom_point() +
  labs(title = "Hello!")
```

Click the "Run cell" button above a chunk to run the code!

![A picture of a chunk of code, with the words "Run cell" at the top.](/.devcontainer/chunk.png)

In groups, we'll try out different variations to see if we can improve a basic plot. If you're not familiar with R code and don't feel confident editing R code, that's okay! The notebook contains different variations with some common changes, and we'll come back together to brainstorm ideas, even if you can't execute them yourself.

### A small note about fonts

To help us make some nice fonts, I've included a font called Inter — it's a nice, free, fairly neutral font. But you may not see it when looking at your plots in the viewer.

There are two ways around this:

1. Save your plot as a PNG file using `ggsave("plot.png", name_of_plot)`
2. [Download Inter from Google Fonts](https://fonts.google.com/specimen/Inter), install it on your computer, and then add `+ theme_grey(base_family = "Inter")` to your plot.
