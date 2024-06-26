# Depraved-Selection

## My depraved way of deciding what movie to watch.

### Why?

Two years ago, I saw what the distribution of release years for movies logged on my Letterboxd looked like. It had an ugly skew to it.

For the past two years, I have kind of become obsessed with reshaping it. After every movie I watch, I refresh the distribution to see how it changed and kind of started watching movies based on if I thought it would make the distribution look prettier.

Earlier this month, I decided I would employ the skills I learned in my data mining class to help scratch the itch of making my distribution look cleaner.

### How it works

First, I export my data from Letterboxd and put the `watched.csv` file in the root of the project directory.

I load the data in with pandas and create a frequency distribution of the release years.
Run polynomial regression on the frequency distribution.

See which years are furthest below from the predicted value of the regression model.

I will then watch a movie from the year furthest below the predicted value on the frequency table, or movies from multiple years that are the furthest below the predicted value.

Once that is done, I will re-adjust the model with the latest data from Letterboxd and do the same thing again.

### Why? (again)

Well... it helps me decide what to watch. Having this kind of structure stops me from being indecisive.

You can check out my Letterboxd account [here](https://letterboxd.com/SpicyMcSpice/).

I also implemented a web scraper that tells me what the most popular movie on my watchlist is from the year with the lowest residual. I sometimes heed the recommendation, sometimes I don't. It feels nice to watch a movie that many people have seen but I haven't. It makes me feel like I'm gaining cultural capital and would be more inclined to get questions right in movie-themed sections of Jeopardy.
