# Bechdel Test

## About This Project
The [Bechdel Test](https://en.wikipedia.org/wiki/Bechdel_test) is test of female representation in fiction. The test is named after American cartoonist Alison Bechdel.

I did some exploratory data analysis of some high level movie data. I was initially inspired by the TedTalk [How Movies Teach Manhood](https://www.youtube.com/watch?v=ueOqYebVhtc&list=PLMDJVgXYlWvjJ-aFkIC1xRmY6pKOP-rEd&index=7), in which Colin Stokes speaks about how movies like the Wizard of Oz has strong female protagonists but later successful movies like Star Wars does not. 

This prompted me to think more about female representation and gender equality in movies in general, and I immediately thought of the Bechdel Test as an easy proxy to help categorize movies. I had a few questions I wanted to answer:
* How many movies in the last 100 years pass the bechtel test?
* What percentage of "top" movies (Oscar Nominees | Oscar Winners | Top 10 grossing movies) pass the Bechdel Test, and is this getting better or worse? 
* Are there certian periods in history that movies passed the Bechdel test even less, and can I find specfiic examples?

## Data

### Bechdel Test Data

I got most of the Bechdel Test ratings from [Bechdel Test Movie List](http://bechdeltest.com/), a crowd-sourced platform of movies and their rating. Mainly, they look at three criteria: 
1. It has to have at least two [named] women in it
2. Who talk to each other
3. About something besides a man
Surprising amoung of movies do not pass even these criteria.

In my data, the `rating` category is based off of these criteria. `3.0` means the movie passed.

I used their [API](http://bechdeltest.com/api/v1/doc).

## Top Movie Data
* I used the [Top 10 Highest Grossing Films (1975-2018)](https://www.kaggle.com/bidyutchanda/top-10-highest-grossing-films-19752018) dataset from Kaggle
* I found the Oscar's Best Pictures nominees and winners on IMDB 

## Tools
* seaborn
* beautifulsoup


# Main Takeaways / Caveats
1. The Bechdel test is not the most comprehensive test for female inclusion in films. In fact, it's the lowest of lowest bars, and many of the movies that technically pass the Bechdel test are far from eschewing themes of gender equality. [FiveThirtyEight](https://projects.fivethirtyeight.com/next-bechdel/) has done great work looking at more useful questions to ask to measure gender imbalance in films. However, it was somehwere I could begin to do some exploratory data analysis with data that already existed, that did not require me to watch hundreds or thousands of films.

2. There was a lot of data missing. Not every single movie was rated on the Bechdel Test Movie List. The movies not rated on Bechdel Test Movie List I unfortunately had to ignore because I did not have the resources to find out whether they passed the Bechdel Test or not.

I'm not sure how much NEW insight I gleaned from this exploratory data analysis, but it was fun to play around with Seaborn charts and to realize that so many movies still do not pass the low bar of the Bechdel Test. 



