
![graph1](./images/NotebookHeader.png)
# Microsoft Movie Optimization Unit

**Authors**: Doug Mill, Carlos McCrum, Seung Lee

## Overview

What Better Way To Launch Microsoft's New Movie Other Than An Original Blockbuster Series?!

Task: Inform Microsoft on how they can premier their first movie successfully. We investigated past movies to see what made the most money and how we can replicate them. We broke down those movies into these categories: What genres are selling, how much money are they spending, and when is the right time to release our movie?


![graph2](./images/director_shot.jpeg)

## Business Problem

Microsoft is looking to launch a movie, however they are unsure of the space. We are here to help visualize what types of movies have been doing well historically and how Microsoft can replicate such success.

By creating our own series, we can create more loyal and dedicated fans, but we must do it right. We first looked through the different genres to see what films attact people and narrow down their interest. Then we wanted looked at the correlation to production budget to gross income, if there was a correlation. Lastly, we look to the seasons to determine the most ideal time to release our movie. 

## Data

The dataset we are using (BigFrame) is derived from 'bom.movie_gross.csv', 'imdb.title.basics.csv', and 'tn.movie_budgets.csv'

BigFrame contains the columns 'release_date', 'movie', 'production_budget', 'worldwide_gross', 'foreign_gross', 'year', 'runtime minutes', and 'genres'. 

To clean BigFrame, we dropped duplicate entries, null values and made it fit our criteria: withtin the last 10 years, production budget of > $1,000,000, and worldwide gross income > $1,000,000. 

This final dataset is N = 967.

This dataframe should give us a good idea of what other large scale movie companies have been doing for to maintain the success.


## Methods

We first prepared the BigFrame by combining all the necessary tables together using a common attribute ('movie'). Next we dropped all unnecessary columns and removed any duplicate entries. 

We then created two columns 'month' and 'year' in order to manipulate the data using time. 'month' to sort the data by seasons within the calender year, and 'year' to sort by the recent timeframe (10years).

## Results

Looking at our results, our recommendation is a well funded (> $100,000,000) Sci-fi / Adverture movie, set to be released in May. 

Releasing our film during May is ideal. History has shown that May returns the greatest revenue income for large production movies. With other movie competition not being so high in the beginning half of the year, May presents itself as the most ideal opportunity to debut our blockbuster film.

### How Well Does Each Genre Perform?
![graph3](./images/genre_domestic.png) ![graph4](./images/genre_foreign.png)

Genres 'Adventure' and 'Sci-fi' returns the highest median gross for movies within our dataset. 'Family' does well domestically, but not too well internationally. 'Action' is also a consistent genre that performs better than average.

### Total Number of Genres Released for Each Genre
![graph5](./images/total_genres.jpg)
Not many production companies are creating Sci-fi films even though they are in high demand. This creates the perfect opportunity for our team.

### Doug's Graphs

![graph6](./images/budget_gross)

![graph7](./images/budget_gross2)

![graph8](./images/budget_gross3)

These graphs demonstrate the correlation between budget and box office performance domestically and worldwide.
Some of the films that had the greatest returns on investment (ROI) were in the $20M-$100M budget range.
Multiple films were able to gain >400% returns domestically and >1000% worldwide.
Budget has a strong positive correlation to box office.
Geographically transcendant films with a budget of <$100M had the greatest ROI (%).
Movies with higher budgets brought in the largest profit margins.

### Seasonal Average Worldwide Gross Income
![graph9](./images/seasonal_gross.jpg)

May is historically the best month for large movie productions. Could be due to summer time and people going on vacations / more free time. Or perhaps because the hot weather encourages more indoor activies. Regardless, summer time is especially attractive time to release our film.

### Number of Movies Released Each Month
![graph10](./images/total_seasonal.jpg)

Combined with the relatively low volume, there is no better time in the year.


## Conclusions

Any skepticism in our data or how we could further explore our dataset (more potentially relevant comparisons)

Sample was 967 movies, ideally we would want that number to be larger.

Go further in depth about how much Sci-Fi and Adventure movies are spending (production_budget) in order to get good returns as shown in Visual 1.

***
Questions to consider:
* What would you recommend the business do as a result of this work?
* What are some reasons why your analysis might not fully solve the business problem?
* What else could you do in the future to improve this project?
***

## For More Information

Please review our full analysis in [our Jupyter Notebook](./dsc-phase1-project-template.ipynb) or our [presentation](./DS_Project_Presentation.pdf).

For any additional questions, please contact **name & email, name & email**

## Repository Structure

Describe the structure of your repository and its contents, for example:

```
├── README.md                           <- The top-level README for reviewers of this project
├── dsc-phase1-project-template.ipynb   <- Narrative documentation of analysis in Jupyter notebook
├── DS_Project_Presentation.pdf         <- PDF version of project presentation
├── data                                <- Both sourced externally and generated from code
└── images                              <- Both sourced externally and generated from code
```
