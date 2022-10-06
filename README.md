# Title

![filmreel](https://github.com/jordanate/phase-1-project/blob/main/images/filmreel.jpeg)

**Author**: Jordana Tepper

**Pace**: Live NYC

**Instructor**: Joseph Mata

## Overview

A one-paragraph overview of the project, including the business problem, data, methods, results and recommendations.

## Business Problem

Microsoft has decided to open a new branch of their company: Microsoft Movie Studios. However, they need help in assessing the different attributes of movies that bring in the most success. Therefore, I have been tasked with aiding the new head of Microsoft Movie Studios in making decisions regarding what type of films to create through the use of data analysis. 

## Data

The data that I used for this analysis comes from two datasets: IMDb and Box Office Mojo. These sources include information about ratings and lengths of various films, genres, directors, actors and actresses, and total gross earnings (foreign and domestic); such data primarily comes from the years 2010 - 2018.

## Methods

Describe the process for analyzing or modeling the data. For Phase 1, this will be descriptive analysis.

***
Questions to consider:
* How did you prepare, analyze or model the data?
* Why is this approach appropriate given the data and the business problem?
***

## Results

Present your key results. For Phase 1, this will be findings from your descriptive analysis.

***
Questions to consider:
* How do you interpret the results?
* How confident are you that your results would generalize beyond the data you have?
***

Here is an example of how to embed images from your sub-folder:

### Visual 1


## Conclusions

This analysis brings about 4 recommendations for Microsoft Movie Studios

1. **The top two genres with the greatest revenue are Action and Adventure.** Although Documentaries tend to be the highest rated genre, ratings do not neccessarily equal success for a business. Rather, revenue is a more appropriate indicator. The genres that clearly had the highest average total revenue (domestic gross + foreign gross) were Adventure movies and Action movies.

2. **Suggested runtime is 101 minutes.** There is no distinct difference in runtime between movies that are rated as 'Good', 'Average', or 'Bad', but if Microsoft Movie Studios is looking for a target runtime, 101 minutes is a good marker as it is the average runtime of 'Good' movies from the two most successful genres: Action and Adventure.

3. **Directors to target are Sam Mendes, Michael Bay, Lee Unkrich, Pierre Coffin, Anthony Russo, and Christopher Nolan**: While there are many successful directors in the film industry, the listed directors have shown to surpass the standard when it comes to the revenue that their movies produce. Not only have these indivudals directed some of the most successful movies in the datasets, but they have also exhibited continuous success throughout the careers.   
4. **Actors to target are Sandra Bullock, Javier Bardem, and Chris Evans**: Similar to the directors presented above, these actors have appeared in the most successful movies from this dataset. Even more so, they have been consistently cast in successful movies throughout the years 2010-2018. Therefore, including such actors in Microsoft films will likely bring in high revenue as well as positive reviews from the audience. 

### Limitations

While these suggestions come from thorough data analysis, there are limitations to this project:

1. **Generalized genres**: Although it may not seem like a surprise that Adventure and Action were observed to be the most successful genres, it is important to note that the genre of each movie in the dataset was generalized. In other words, many movies had multiple genres listed, but for the sake of analysis, one genre had to become the primary genre. To do so, I took the first genre listed and made it the primary genre for a given movie. Moreover, when a movie had multiple genres, they were listed in alphabetical order making Adventure and Action often come first and serve as the primary genre. While this may seem like a significant issue, I support this decision for two reasons. First, when looking at the number of movies per genre after assigning each movie a primary genre, Action and Adventure do not hold monopolies over the dataset. In fact, neither genre is in the top three genres with the most movies. Second, I believe that Adventure and Action do tend to be overarching genres meaning that even if a movie is listed as Action and Drama or Adventure and Comedy, the movie can safely be categorized as Action and Adventure, respectively.

2. **Recency of data**: As mentioned, much of the data from this analysis comes from 2010 - 2018. Therefore, this project lacks information from the past four years. However, I do not believe that this weakens my project because two out of the last four years were largely inmpacted by COVID-19. In other words, the field of movie production in 2020 and 2021 was not an accurate representation of how movies will be made in the upcoming years. While COVID-19 has made irreversible changes to our world, I think that future movie production is more likely to resemble how it was pre-COVID than how it was _during_ COVID.

### Further Questions

1. What is the best form of advertising a movie?
2. How do we bring in the suggested directors and actors?
3. Is it better to release a movie on streaming platforms (ex: Netfix, Hulu, HBO Max) or in theaters? Which streaming platform would be best?

***


## For More Information

For a full analysis please look at my [Jupyter Notebook](./phase-1-project-notebook.ipynb) or review my [presentation](./).

For any additional questions, please contact Jordana Tepper at jtepper724@gmail.com

## Repository Structure:

```
├── README.md                           
├── phase-1-project-notebook.ipynb   
├── .pdf         
├── zippedData                                
└── images                              
```
