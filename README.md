# Phase 1 Project: Movie Analysis for Microsoft Movie Studios

![filmreel](https://github.com/jordanate/phase-1-project/blob/main/images/filmreel.jpeg)

**By**: Jordana Tepper

## Overview

This project analyzes existing movie data in order to help Microsoft with the launch of its new production studio. Such data consists of movie ratings, cast and crew, gross earnings, and movie runtime. After utilizing the process of exploratory data analysis, I provide four recommendations for Microsoft Movie Studios, including the most successful genres, the ideal length of a movie, and target directors and actors.

## Business Problem

Microsoft has decided to open a new branch of their company: Microsoft Movie Studios. However, they need help in assessing the different attributes of movies that bring in the most success. Therefore, I have been tasked with aiding the new head of Microsoft Movie Studios in making decisions regarding what type of films to create through the use of exploratory data analysis. 

## Data

The data that I use for my analysis comes from two datasets: IMDb and Box Office Mojo. These sources include information about ratings and lengths of various films, genres, directors, actors and actresses, and total gross earnings (foreign and domestic); such data primarily comes from the years 2010 - 2018.

## Methods

This project includes thorough data cleaning, such as removing entries with missing values and combining various columns from two different datasets to create new, more explicit, DataFrames. Furthermore, I utilize different types of graphs to adequately present the findings from this data analysis.

## Analysis

### Average Rating Per Genre

For my first analysis, I look at the average movie rating per genre using a bar chart. I also include a color scale to show the number of ratings that each genre received in order to add another level of understanding to the graph.

![rating_x_genre.png](https://github.com/jordanate/phase-1-project/blob/main/images/rating_x_genre.png)

### Total Revenue Per Genre

After looking at my first analysis, I realize that from a business point of view, success is not determined by ratings, but rather, it is indicated by revenue.

Therefore, for the subsequent analysis, I look at the average total revenue per genre using a bar graph.

![revenue_x_genre.png](https://github.com/jordanate/phase-1-project/blob/main/images/revenue_x_genre.png)

### Distributions of Runtimes For Action and Adventure Movies Based on Rating Category

In the next analysis, I look at the distribution of runtimes for Action and Adventure movies using boxplots. I do so for each individual rating category ('Good', 'Average', and 'Bad'), resulting in three separate boxplots - each with two diagrams (one for Action, one for Adventure).

The rating categories are determined based on the following criteria:

* 'Good' means a movie rating greater than or equal to 7
* 'Average' means a movie rating of less than 7 and greater than or equal to 5
* 'Bad' means a movie rating of less than 5

![distribution_runtimes.png](https://github.com/jordanate/phase-1-project/blob/main/images/distribution_runtimes.png)

### Directors of the Most Successful Movies

During this analysis, I examine and graph the top 15 directors whose movies produced the greatest mean revenue in 2010-2018, as well as the directors of the top 15 movies with the greatest single revenue in 2010-2018.

After, I compare the two graphs and look at the directors who appear in both graphs. While doing so, I am attentive to the fact that some directors appear in both graphs because they directed one particularly successful movie resulting in the mean revenue of the movies they directed seeming very high. Therefore, I consider the most successful directors to be only the individuals who are present in both graphs *and* who have directed more than one movie in 2010-2018.

![directors_spaced.png](https://github.com/jordanate/phase-1-project/blob/main/images/directors_spaced.png)

### Actors and Actresses from the Most Successful Movies

In my final analysis, I do a process very similar to what I did with the directors. I examine and graph the top 15 actors whose movies produced the greatest mean revenue in 2010-2018, as well as the actors from the top 15 movies with the greatest single revenue in 2010-2018.

Next, I compare the two graphs and look at which actors appear in both graphs. As I did in the previous analysis, I pay close attention to the fact that some actors appear in both graphs because they were in one particularly successful movie making the mean revenue of the movies they were in seem very high. Therefore, I consider the most successful actors to be only the individuals who are present in both graphs *and* who were cast in more than one movie in 2010-2018.

![actors_spaced.png](https://github.com/jordanate/phase-1-project/blob/main/images/actors_spaced.png)

## Conclusions

This data analysis brings about 4 recommendations for Microsoft Movie Studios.

1. **The top two genres with the greatest revenue are Action and Adventure.** Although Documentaries tend to be the highest-rated genre, ratings do not necessarily equal success for a business. Rather, revenue is a more appropriate indicator. The genres that clearly had the highest average total revenue (domestic gross + foreign gross) were Adventure movies and Action movies. Therefore, Microsoft Movie Studies should aim to produce films of these genres.


2. **Suggested runtime for Action movies is between 85 and 125 minutes.** There is no distinct difference in the mean runtime between movies that are rated as 'Good', 'Average', or 'Bad', but if Microsoft Movie Studios is looking for a target runtime range, within 85 and 125 minutes for Action movies is ideal; to be even more specific, a runtime of 100 minutes would be a solid target length (such information comes from the runtime distribution of 'Good' Action movies). It is more difficult to give a suggestion for Adventure movies as the distributions for 'Good', 'Average', and 'Bad' movie lengths are all quite similar. Nevertheless, in regard to Action movies, aiming within the specified range maximizes the likelihood of audience approval.


3. **Directors to target are Sam Mendes, Michael Bay, Lee Unkrich, Pierre Coffin, Anthony Russo, and Christopher Nolan**: While there are many successful directors in the film industry, the listed directors have shown to surpass the standard when it comes to the revenue that their movies produce. Not only have these individuals directed some of the most successful movies in the datasets, but they have also exhibited continuous success throughout their careers, making them reliable in regard to bringing in revenue. The ideal directors for Action movies are Sam Mendes, Michael Bay, and Anthony Russo, and the ideal directors for Adventure movies are Lee Unkrich and Pierre Coffin. The director that has experience in both genres is Christopher Nolan.
   

4. **Actors to target are Sandra Bullock, Javier Bardem, and Chris Evans**: Similar to the directors presented above, these actors have appeared in the most successful movies from this dataset. Even more so, they have been consistently cast in successful movies throughout the years 2010-2018. Therefore, including such actors in Microsoft films will likely bring in high revenue as well as positive reviews from the audience. In terms of specific genres, Chris Evans and Javier Bardem are both known for Action movies, while Sandra Bullock has experience in both Action and Adventure movies. 


### Limitations

While these suggestions come from thorough data analysis, there are limitations to this project:

1. **Generalized genres**: Although it may not seem like a surprise that Adventure and Action were observed to be the most successful genres, it is important to note that the genre of each movie in the dataset was generalized. In other words, many movies had multiple genres listed, but for the sake of analysis, one genre had to become the primary genre. To do so, I took the first genre listed and made it the primary genre for a given movie. Moreover, when a movie had multiple genres, they were listed in alphabetical order making Adventure and Action often come first and serve as the primary genre. While this may seem like a significant issue, I support this decision for two reasons. First, when looking at the number of movies per genre after assigning each movie a primary genre, Action and Adventure do not hold monopolies over the dataset. In fact, neither genre is in the top three genres with the most movies. Second, I believe that Adventure and Action do tend to be overarching genres meaning that even if a movie is listed as Action and Drama or Adventure and Comedy, the movie can safely be categorized as Action and Adventure, respectively.

2. **Recency of data**: As mentioned, much of the data from this analysis comes from 2010 - 2018. Therefore, this project lacks information from the past four years. However, I do not believe that this weakens my project because two out of the last four years were largely impacted by COVID-19. In other words, the field of movie production in 2020 and 2021 was not an accurate representation of how movies will be made in the upcoming years. While COVID-19 has made irreversible changes to our world, I think that future movie production is more likely to resemble how it was pre-COVID than how it was _during_ COVID.

### Further Questions

1. What is the best way of advertising a movie?
2. How do we bring in the suggested directors and actors?
3. Is it better to release a movie on streaming platforms (ex: Netflix, Hulu, HBO Max) or in theaters? Which streaming platform would be best?

***


## For More Information

For a full analysis, please look at my [Jupyter Notebook](./phase-1-project-notebook.ipynb)
<br /> For a more concise summary, please review my [presentation](https://github.com/jordanate/phase-1-project/blob/main/Phase%201%20Project%20Presentation.pdf).

<br />
For any additional questions, please contact Jordana Tepper at [jtepper724@gmail.com](mailto:jtepper724@gmail.com) 

## Repository Structure:

```
├── README.md                           
├── phase-1-project-notebook.ipynb   
├── Phase 1 Project Presentation.pdf         
├── zippedData                                
└── images                              
```
