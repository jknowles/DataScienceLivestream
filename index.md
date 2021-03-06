---
layout: page
title: Jared's Data Science Livestream
tagline:
description: Watch a data scientist at work
---

### When is the next stream?

The data science livestream is taking a break while I am on vacation. Streams
will resume on Monday 10/24/2016.

Check out my [Twitter account for updates](http://www.twitter.com/jknowles).

### Where can I find it?
[YouTube Channel](https://www.youtube.com/user/debatemanjk)

### Where can I learn more?

You can learn about what the project I'm working on is [here](pages/project.html).
You can see why I'm streaming [here](pages/whystream.html) and you can have
some other questions answered over on the [FAQ](pages/faq.html).

### What's the latest?

Here I'll catch you up on my progress so when you tune in you can see what I've
done and where I'm at for the day.

#### 10/07/2016

Unfortunately the livestream is canceled. The internet is not reliable today
and my uplink is too slow to stream.

#### 10/06/2016

A little EDA.

#### 10/05/2016

More investigation of data problems and validation against published figures. I
do some EDA on the arrest data to check my understanding and identify possible
tests I can write to validate my ETL process.

#### 10/04/2016

I talk about slow data analysis and the upside of methodically working through
simple problems in the data to increase understanding and fluency with the
basic foundations of the data set. I identify some big holes in the data and
discuss where other potential reporting errors/inconsistencies might be hiding.
I talk about why it is critical to seek these out.

#### 10/03/2016

Back on track I dig back into the data to try to validate my data sources by
recreating publicly published statistics from the FBI. I discuss the issues
with how the data was collected and talk about how understanding the data
generation process helps to diagnose potential issues with your understanding
of the data and how to check them.

#### 09/30/2016

After setting up my new data architecture that includes a PostGres database
running in a Docker container, I talk about how to ETL data into a database and
work through parsing the data I have from the FBI on arrests. I do some
data inspection, data cleaning, and writing and reading from the database.

#### 09/29/2016

I showed off the new architecture using a Ubuntu Server virtual machine, a
Postgres database running in a docker container, and RStudio server. I then
talked about ETL work and the thinking through of how to organize raw data
into tables in the database for querying. I then showed a bit of my ETL
workflow and talked about deduplicating data before writing it to the database.

#### 09/28/2016

I find some new data on arrests that is necessary to recreate the FBI reports.
I show how to organize that data and how to modify code to ingest that data
into R and store in a SQLite database.

#### 09/27/2016

Instead of boring everyone with my head scratching I spent the day diving deeper
into data definitions and exploring some of the data requirements.

#### 09/26/2016

I plan on trying to recreate some basic calculations from the FBI's Crime in
United States report series which uses UCR data to report on trends in national
and state crime levels in the United States.

#### 09/23/2016

Started some exploratory data analysis. I looked at basic calculations of
crime rates per population and I looked for reporting errors and outliers in
reporting by year, by state, and by month using both graphs and summary
statistics.

I also started thinking about how to recreate FBI reported crime rates to
calibrate my understanding of the data.

#### 09/22/2016

Continuing the data cleaning theme today I am going to write code that identifies
agencies that have their data reported by another agency. I will look at the
different ways this occurs in the data (within year, across years, etc.) and
then I will write some functions to clean this in different ways that I can
apply when needed.

#### 09/21/2016

Today I investigated the missing data flags in the dataset to apply
custom rules for different missingness patterns. I specifically identified
when only a few arbitrary months of data were missing and reconciled the case
where that data is not reported at all and cases where the data is included in
another month of reporting.

This involved a lot of EDA work and some careful use of conditional and
logical statements to come up with strong business logic that captures different
cases. I also wrote a few more cleaning functions using `dplyr`.

#### 09/20/2016

On the stream today I worked on writing functions to interpolate data where an
agency reported crime data annually or bi-annually. I built a function to fit
a model to model month to month trends and then spread the annual data out
across the months using that model.

I used a lot of `dplyr` and learned how to combine `mutate` and `mutate_` calls
effectively to work with static and dynamic variable names within a pipeline.

The stream itself was not that great -- I'm still working the bugs out on how to
cast the screen at high enough resolution. I also need to do a little more talking
to the audience and explain my thought process out loud occasionally.
