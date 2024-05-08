DSC 200 Lab Project -Term 2232
================
2024-05-08

**Student Name:<insert your name here>**

**Student ID:<insert ID here>**

**Deadline:** 23:59 on Sunday, 19 May 2024

**Total Points:** 20

## Loading Packages

``` r
library(tidyverse)
library(openintro)
library(ggrepel)
```

## Tasks

\`1. (2 points)

Write your narrative here

\`2. (2 points)

Write your narrative below

\`3. (2 points)

Write your narrative here

\`4. (2 points)

Write your narrative here

\`5. (2 points)

Write your narrative here

\`6. (2 points)

Write your narrative here

\`7. (2 points)

Write your narrative here

\`8. (2 points)

Write your narrative here

\`9. (2 points)

The code below selects the records of the ten most common pet names and
assigns them to the variable top_10_names. (Refer to Task4 above).

``` r
top_10_names <- seattlepets %>% 
filter(animal_name %in% c( "Lucy"  , "Charlie" , "Luna" , "Bella" , "Max"    , 
                           "Daisy" , "Molly"   , "Jack" , "Lily"  , "Stella" ))
top_10_names
```

    ## # A tibble: 2,974 × 7
    ##    license_issue_date license_number animal_name species primary_breed          
    ##    <date>             <chr>          <chr>       <chr>   <chr>                  
    ##  1 2018-11-25         S120480        Charlie     Dog     Retriever, Labrador    
    ##  2 2018-11-03         829563         Max         Dog     Retriever, Labrador    
    ##  3 2018-10-29         732106         Lily        Cat     Domestic Shorthair     
    ##  4 2018-11-25         895808         Max         Cat     Domestic Shorthair     
    ##  5 2018-11-26         834841         Daisy       Dog     Terrier, American Pit …
    ##  6 2018-12-13         8003804        Charlie     Dog     Border Collie          
    ##  7 2018-11-06         S125292        Jack        Cat     Domestic Shorthair     
    ##  8 2018-11-01         835179         Stella      Dog     Retriever, Labrador    
    ##  9 2018-12-14         950094         Molly       Dog     Retriever, Labrador    
    ## 10 2018-11-24         S137301        Lucy        Dog     Hound                  
    ## # ℹ 2,964 more rows
    ## # ℹ 2 more variables: secondary_breed <chr>, zip_code <chr>

\`Plot the counts of the pet names (animal_name) in top_10_names

\`10. (2 points)

\`The below code plots the proportion of dogs with a given name versus
the proportion of cats with the same name. The 20 most common cat and
dog names are displayed. The diagonal line on the plot is the x = y
line; if a name appeared on this line, the name’s popularity would be
exactly the same for dogs and cats.

    ## Warning: Using `size` aesthetic for lines was deprecated in ggplot2 3.4.0.
    ## ℹ Please use `linewidth` instead.
    ## This warning is displayed once every 8 hours.
    ## Call `lifecycle::last_lifecycle_warnings()` to see where this warning was
    ## generated.

    ## Warning in geom_image(mapping, data, inherit.aes = inherit.aes, na.rm = na.rm, : All aesthetics have length 1, but the data has 20 rows.
    ## ℹ Please consider using `annotate()` or provide this layer with data containing
    ##   a single row.
    ## All aesthetics have length 1, but the data has 20 rows.
    ## ℹ Please consider using `annotate()` or provide this layer with data containing
    ##   a single row.

![](Lab_project_files/figure-gfm/unnamed-chunk-11-1.png)<!-- -->

\`What names are more common for cats than dogs? The ones above the line
or the ones below the line?

\`Answer here………………

\`Is the relationship between the two variables (proportion of cats with
a given name and proportion of dogs with a given name) positive or
negative? What does this mean in context of the data?

\`Answer here ………….
