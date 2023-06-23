Vignette Blog Post
================
Jessica Ayers
2023-06-22

``` r
rmarkdown::render("/Users/jessayers/Documents/ST 558/TOPIC 2/blog/_Rmd/2023-06-22-my-new-blog-post.Rmd",
output_format = "github_document",  
output_dir = "/Users/jessayers/Documents/ST 558/TOPIC 2/blog/_posts" ,
output_options = list(html_preview = FALSE))
```

## Vignette Blog Post

### Explanation of Project & Interesting Findings

I used the Open Movie Database API (omdbapi) to create my vignette. In
the project, I created a function to return both a single random movie
and a data frame with 10 random movies. The theme of the project was
movies with different colors in the titles. The options provided were
blue, red, and green along with years of 2000, 2010, 2020. There were 9
combinations of possible results. For the exploratory data analysis,
only the data frames were used as more movie titles were returned from
the API. Each call using the search and year parameters for the omdbapi
returned only 10 titles. Three data frames were combined from each of
the available years in the created function. It was found that the data
base contained games, movies, and tv series with very few sequels. Since
only character data was returned from the api in the form of a data
frame, a numerical variable representing the length of the title was
created. Contingency tables, numerical summaries, and plots were created
to describe the data in different ways.

### Reflection

Overall, I found this project very beneficial in improving my API and
GitHub skills. It took some time to figure out how to get the omdbapi to
return actual data. At first it was only returning a single movie at a
time. With summaries and plots as the end goal, having one data point is
not very efficient. After a while I was able to get the API to return 10
movies at a time. This was something I could work with! Connecting the
API and having it return multiple movie titles was the most difficult
part in beginning this project. Another situation that caused some
difficulty was that the data frames only returned character data. It
gave the title, year, imdbID, and type of program. When searching for a
specific title, the API returned a single random movie. More data was
provided with that output, but a single data observation is not
something that can easily be worked with. The most difficult programming
piece was the inclusion of for loops in creating the two new variables.
When approaching a similar project in the future, I would make sure that
the API I am working with is outputting exactly what kind of data I need
to do further analysis.

### Links

[GitHub Pages Repo](https://jessicaayers.github.io/Project-1)

[Regular Repo](https://github.com/jessicaayers/Project-1.git)
