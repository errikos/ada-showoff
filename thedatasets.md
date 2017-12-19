---
layout: page
title: The datasets
subtitle: A few words on the datasets used
---

## General Info

We use two datasets in this analysis:
  1. The so-called "Tweets Leon" database, which was kindly provided by EPFL (restricted access).
  2. A collection of tweets tweeted from Switzerland, obtained via <a href="https://twitter.com/sp3r" target="_blank">Spinn3er</a>.

**Tip:** You can hover on the graphs to see additional info and insights.

## Tweets Leon

The Tweets Leon database consists of about **18 billion tweets**, made between October 2010 and January 2016. That is about **5 years** worth of tweets.

The available metadata (columns) of this dataset were:
  - Language
  - Tweet ID
  - Date and time of posting
  - Username
  - Text

Therefore, we were unfortunately not able to conduct any analysis based on the location of the users. But we can still do other interesting stuff!

#### Language distribution

The following plots show the language distribution of the Tweets Leon database.

As expected, the majority of tweets is in English, with Spanish following well behind. Despite the rest of the languages having around half a billion tweets each, their sum does not even reach the Spanish tweets count.

{% include plots/leon/leon_lang_bar.html %}
{% include plots/leon/leon_lang_pie.html %}

#### Monthly distribution

The graph below shows the monthly distribution of tweets in the dataset. While the dataset specification states that the tweets should span from June 2013 to January 2016, we can see that there are a lot of tweets from 2011 and 2012 as well. Given that the timestamps are correct, this is a good thing for our analysis, as we get to see the impact of older events as well (yay!).

{% include plots/leon/leon_monthly.html %}

One thing to keep in mind here is that the tweets in the dataset make up only a fraction (about 10%, as per the metadata) of the actual tweets written during that period. As the only indication we have is that "the tweets are not filtered", we shall assume that sampling was done in a random manner, thus it does not bias the results.

## Swiss Tweets

The Swiss Tweets database consists of about 11 million tweets, made between 2016-01-01 and 2016-10-31. That is 10 months worth of tweets.

#### Language distribution

In the following plots you can see the language distribution for the Swiss tweets database. We decided to only include the languages which also exist in the Tweets Leon dataset, that is (in descending count order): English, Spanish, German, French, Italian and Dutch.

{% include plots/swiss/swiss_lang_bar.html %}
{% include plots/swiss/swiss_lang_pie.html %}

Surprisingly (or not) enough, **most of the tweets are in English** which indicates the impact the latter has as a language. Notably, the tweets in English are as many as the tweets in French and German, combined. Once again, we see a **fairly high amount of tweets in Spanish**, surpassing the tweets written in Italian, which is one of the official languages of Switzerland.

#### Daily distribution

As one can see in the graph below, the daily count of tweets remains relatively constant, in the sense that there are no steep ups and downs. Of course, from August and later, the available tweets seem to triple in count. Since we had no control over the dataset sampling, we will just have to live with it!

{% include plots/swiss/swiss_daily.html %}

**Note:** We chose to show the daily distribution for the Swiss Tweets dataset, because the period in which the tweets span is relatively short.

## Comments

#### Non-overlapping periods

As you can see, **the intersection of the periods** that are covered by each dataset **is practically non-existent**. This is a pity, because it disables any comparative analysis that could be done for the same set of events between the tweets made from Switzerland vs. the rest of the world.

Therefore, our analysis focused on how the world and Switzerland reacted to the events that took place within each individual period, i.e. from October 2010 until January 2016 and from January 2016 until October 2016, respectively.
