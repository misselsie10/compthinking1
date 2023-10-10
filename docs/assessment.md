
# TEAM PORIFERA ASSESSMENT

## Q1

Match the following types of real-world data to their equivalent R type and explain your reasoning.

-   Real world data: scientific names, the count of plants in a quadrat, whether or not it rained on a sequence of days, and the reaction times of birds to disturbances in seconds

-   R types: logical, integer, numeric, and character

## ANSWER:

logical = whether or not it rained on a sequence of days

integer = the count of plants in a quadrat

numeric = the reaction times of birds to disturbances in seconds

character = scientific names

------------------------------------------------------------------------

## Q2

Use this code chunk to answer the following questions.

```         
bird_mass_g <- c(100.1, 99.2, 99.3, NA, 100.0, 101.5, 94.7, 99.2, 108.2)
mean_mass <- mean(bird_mass_g)
sd_mass <- sd(bird_mass_g)
is_outlier <- bird_mass_g > mean_mass + 3 * sd_mass
num_outliers <- sum(is_outlier)
```

-   In plain english, what does this code chunk do?

-   Two of the lines have mistakes that keep the code from doing what it's supposed to. What are the mistakes and how would you fix them?

-   What are the types of `bird_mass_g`, `is_outlier`, and `num_outliers`?

## **ANSWER:**

The first line of the code assigns a data frame (mass of birds in grams) to bird_mass_g.

The second line of code assigns the calculated mean of the data frame to be mean_mass.

The third line of code assigns the calculated standard deviation of the bird mass data to be sd_mass.

The fourth line of code assigns any mass within the data that is 3 standard deviations away from the mean to be assigned to the data frame is_outlier.

The fifth line of code calculates the sum of the outliers to be assigned num_outliers.

------------------------------------------------------------------------

## **Q3**

How could you change the first line of code in the following chunk so that `median_count` comes out to `5L`?

```         

quad_counts <- c(2L, 19L, 4L, 5L, 5L, 12L, 0L, 7L)
valid_quads <- c(1, 2, 3, 5, 7) 2,19,4,5,0 0,2,4,5,19
quad_counts2 <- quad_counts[valid_quads]
median_count <- median(quad_counts2)
```

## ANSWER:

I would change the first line of code to be in numerical order as such:

quad_count \<- c(0L, 2L, 4L, 5L, 5L, 7L, 12L, 19L)
