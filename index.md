---
layout: page
title: Tweeting Events
subtitle: An event-based analysis of Tweets around the world
use-site-title: true
---

# Introduction

In this analysis we are going to show some interesting results that we found out by analysing Tweets from Switzerland and all over the world. To find out more about the datasets and their characteristics, please consult the [datasets page]({{site.baseurl}}/thedatasets).

The first step was to run back in time and distinguish about 70 events that took place around the world, spanning from January 2011 to October 2016. These events vary, from natural disasters (e.g. the Japan earthquake in 2011) and terrorist attacks (e.g. the Paris attacks in 2015) to political situations (e.g. Egyptian revolution in 2011) and deaths of well-known people (e.g. Robbin Williams suicide in 2014).

We then went through the datasets and collected the amount of tweets that were made daily and which "matched" each one of the defined events. This information was more than enough to conduct our analysis.

#### Disclaimer

The following analysis was done as part of the ADA course @ EPFL and while doing it we were trying to also have fun. Some of the comments made below are meant to be taken as humourous ones and do not necessarily reflect the authors' individual opinions.

Furthermore, at no point we do imply that event X is more significant than event Y. The only variable of the comparison in each case is the event's impact on Twitter and nothing more.

# Part I: Swiss Tweets

The Swiss Tweets database is the smaller of the two and it spans just ten months, from January 2016 until (and including) October 2016. To compensate for that, the database includes sentiment data for each tweet, which we will use below.

## Events of 2016

For 2016, we distinguished 15 events by focusing mainly on Europe. We also included some main global events, that could have made an impact on people living in Switzerland.

* Zika virus outbreak (28th January)
* North Korea rocket launch (7th February)
* North Korea nuclear test (9th September)
* Obama visit to Cuba (21st March)
* EgyptAir flight 804 crash (19th May)
* UK referendum to leave the EU (23rd June)
* Ataturk Airport attack (28th June)
* Juno enters Jupiter orbit (5th July)
* Turkey coup attempt (15th July)
* Olympic Games in Rio, Brazil (August)
* Panama papers (3rd April)
* Pokemon Go! (July)
* Montreux Jazz Festival 2016 (April)
* Brussels Airport attack (22nd March)
* Nice Bastille day attack (14th July)
* Burkini ban in France (January)

## Analyzing reactions...

At this point we will demostrate some of the facts we derived from the data. Keep in mind that the tweets in the dataset are only a fraction of the total tweets made at that period.

### A game vs. a serious matter

Do you remember Pokèmon from your childhood? Well, even if you didn't, Niantic reminded us in 2016 by creating a mobile game based on these beloved (or not) little creatures. The game was a major hit. But how much of an impact it had?

It turns out quite a lot. And we can say that because it's effect is analogous to that of the "Burkini Law" that was passed in France, at roughly the same period.

{% include plots/swiss/counts_go_vs_burkini.html %}

Pokèmon Go! was officially released in Europe in 6th July 2016, however it's development had started since 2014. In early 2016 one could download and try beta versions of the game and watch videos online, thus the sparkle in tweets from March 2016.

On the other hand, the Burkini discussion in France did not begin until August. We can see that, even though the discussion attracted interest for about half a month, this interest faded rather quickly, while the interest in Pokèmon Go! remains quite steady during September and October.

### A concert timeline

The Montreux Jazz Festival is an annual music festival, which takes place in Montreux, Switzerland. It is the second largest annual jazz festival in the world after Canada's Montreal International Jazz Festival.

The graph below shows the number of tweets referring to the festival during 2016. Based on the graph, can you identify the events that happened at each moment in time?

{% include plots/swiss/counts_montreux.html %}

By looking at the almost-continuous region in the beginning of July one can guess that this is the period when the festival took place. This is because of the peak in interest in the beginning of the aforementioned period (everyone is excited at the beginning) and also due to the length of the period (such festivals last about 2-3 weeks).

If you look at the pattern of interest, it makes sense, as the most popular days of such events are the first and the last days (when everyone wants the event to never end).

But how about that peak in April? It turns out that on 14th April, the ticket sale for the festival started! Our timeline gives away all this information perfectly. See you in the festival next year!

### North Korea is as popular as chocolate

No kidding. Of course, year 2016 was one in which North Korea drew a lot of attention from the global community. We expected for it to be discussed in Switzerland as well. But for the country to be almost as popular as chocolate, in Switzerland, that is really interesting and amazing!

{% include plots/swiss/counts_nkorea_chocolate.html %}

We believe that Swiss people should tweet more about their amazing chocolates!

### Referendums are cool

On 23rd June 2016, all attention was drawn to the United Kingdom and its referendum to remain to or leave from the European Union. Once again, people (living in Switzerland) showed that they enjoy making political decisions (or in this case watching others make political decisions!).

{% include plots/swiss/counts_brexit_power.html %}

The interest in the UK referendum tops, in absolute value of tweets, any other event that we tracked, beating the next most popular event, the Summer Olympics in Rio by double score.

### Cumulative plot

We leave you a cumulative plot to play with. Click [here]({{site.baseurl}}/swiss_all) for the full-screen plot.

{% include plots/swiss/counts_all.html %}

## Tell me how you feel

The Swiss Tweets dataset also contained a field "sentiment" for the majority of the tweets. Using it, we were able to find some interesting stuff about the tweets resembling to each event.

{% include plots/swiss/sentiment_swiss_all.html %}

We were happy to see that in most cases the polarity of the tweets matches the expected sentiment for the corresponding event.

There are however some events for which the reactions have mixed feelings. The most "dividing" topic seems to be the visit of President Obama to Cuba, for which ~57% of the tweets in the sample have positive feelings and ~43% of them have mixed feelings.

And of course there is the UK referendum, for which about ~60% of the tweets have negative feelings, while ~40% of them have positive ones.

# Part II: Tweets Leon

We will begin by listing the events on which we based our analysis for the Tweets Leon database, as well as our basic findings for each category. The Tweets Leon database roughly spans from January 2011, until December 2015.

## Reaction on well-known people deaths

We begin by presenting our findings regarding the Twitter's reaction to the deaths of well-known people. We tried to include well-known people from a variety of topics, such as politics, technology, artists, etc., as well as from various regions of the world.

Let us list the well-known people, for which we collected data:
* [Steve Jobs](https://en.wikipedia.org/wiki/Steve_Jobs) (5th October 2011)
* [Kim Jong-il](https://en.wikipedia.org/wiki/Kim_Jong-il) (17th December 2011)
* [Amy Winehouse](https://en.wikipedia.org/wiki/Amy_Winehouse) (23rd July 2011)
* [Whitney Houston](https://en.wikipedia.org/wiki/Whitney_Houston) (11th February 2012)
* [Neil Armstrong](https://en.wikipedia.org/wiki/Neil_Armstrong) (25th August 2012)
* [Nelson Mandela](https://en.wikipedia.org/wiki/Nelson_Mandela) (5th December 2013)
* [Paul Walker](https://en.wikipedia.org/wiki/Paul_Walker) (30th November 2013)
* [Robin Williams](https://en.wikipedia.org/wiki/Robin_Williams) (11th August 2014)
* [John Forbes Nash](https://en.wikipedia.org/wiki/John_Forbes_Nash_Jr.) (23rd May 2015)
* [Christopher Lee](https://en.wikipedia.org/wiki/Christopher_Lee) (7th June 2015)
* [Lemmy](https://en.wikipedia.org/wiki/Lemmy) (28th December 2015)

{% include plots/leon/counts_well_known_deaths.html %}



## Reaction on loss of life

By "mass loss of life" we mean any event, natural or man-provoked event that leads to a large amount of people losing their life. For example, natural disasters, like earthquakes and tornadoes and any form of violence (e.g. suicide bombings) belong to this category.

For reference, we list the events we selected for analysis:
* Japan Earthquake & Tsunami (March 2011)
* Egyptian Revolution, Hosni Mubarak resignation (February 2011)
* Egyptian coup against Mohamed Morsi (July 2013)
* New-Zealand earthquake (February 2011)
* Mark Duggan police killing, UK riots (August 2011)
* Houla Massacre in Syria (May 2012)
* Oscar Pistorius murders his girlfriend (February 2013)
* Boston Marathon bombing (April 2013)
* Ghouta, Syria sarin gas attack (August 2013)
* Ebola outbreak in West Africa (December 2013)
* Malaysian Airlines MH370 disappears (May 2014)
* Malaysian Airlines MH17 shot down (July 2014)
* Peshawar school massacre in Pakistan (December 2014)
* Ferguson shooting (August 2014)
* Charlie Hebdo attack In Paris (January 2015)
* Germanwings plane crash (May 2015)
* Garissa University College shooting in Kenya (April 2015)
* Nepal magn. 7.8 and 7.3 earthquakes (April 2015)
* Ankara bombings (October 2015)
* Paris terrorist attacks (November 2015)

{% include plots/leon/counts_loss_of_life.html %}

## Reaction on scientific and political events

Scientific events consist of events that are related to the scientific world and technological world.

* Higgs Boson discovery (4th July 2012)
* Curiosity Lands on Mars (6th August 2012)
* Felix Baumgartner sky-dive (Red Bull Stratos) (14th Octover 2012)
* Shenzhou 9 Chinese spacecraft dock (18th June 2012)
* Edward Snowden, NSA (20th May 2013)
* Pope Francis election (13th May 2013)
* Scotland UK referendum (18th September 2014)
* Rosetta lands on comet (12th November 2014)
* Greek government-debt crisis (June 2015)
* Cuba and USA reestablish diplomatic relations (20th July 2015)
* Volkswagen scandal (September 2015)
* Climate change pact in Paris (13th December 2015)
* SpaceX lands Falcon 9 (22nd December 2015)

{% include plots/leon/counts_science_politics.html %}

## Reaction on sports events

Sport-related events always catch public attention. We decided to include only main events, such as the FIFA World Cup (football) and the Olympic Games. There are two main events during our period, specifically:

* 2012 Olympic Games in London (Summer 2012)
* 2014 FIFA World Cup in Brazil (Summer 2014)

{% include plots/leon/counts_sports.html %}

## Reaction to non-significant events

By "non-significant" we simply mean gossip events, that is, events that would have no impact in one's life even if they had never heard of them (so don't feel bad if you haven't)!

* Royal Wedding (UK) (29th April 2011)
* Doomsday - 31st December 2012 (December 2012)
* Harlem Shake (February 2013)
* North West (Kim Kardashian + Kanye West) (15th June 2013)
* #BreakTheInternet by Kim Kardashian (12th November 2014)

{% include plots/leon/counts_other.html %}

Wow, it seems that a wedding of the Royal Family, is as popular as an impending end of the world! Who knew...

## Some interesting observations

When starting this project, we were expecting that the "non-significant" events would attract all of the interest of Twitter. And this would not be a bad thing, after all we can't always discuss or read about things that make us sad. On the other side, it is always nice to not get carried away.

We are happy that this is not the case, however we can see that there is a trend:
* For more serious events, the public* attention seems to sparkle immediately, but it fades rather quickly. However, it will sparkle again, if new things happen regarding the aforementioned event.
* For more "gossipy" events, the public attention will sparkle equally fast, it will fade rather quickly, but it will be very difficult to respawn. E.g. the Harlem Shake was forgotten pretty quickly.

* By public we mean the sample public.


### Cumulative plot

We leave you a cumulative plot to play with. Click [here]({{site.baseurl}}/leon_all) for the full-screen plot.

{% include plots/leon/counts_all.html %}