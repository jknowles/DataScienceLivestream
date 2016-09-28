---
layout: page
title: Jared's Data Science Livestream
tagline:
description: Watch a data scientist at work
---

### When is the next stream?

For the week of 09/26/2016 the plan is to stream:

- 09/26 - 9:30am - 11:30am Eastern (1:30pm - 3:30pm UTC)
- 09/27 - 9:30am - 11:30am Eastern (1:30pm - 3:30pm UTC) (DELAYED)
- 09/28 - 9:30am - 11:30am Eastern (1:30pm - 3:30pm UTC)
- 09/29 - 1:30pm - 4pm Eastern (5:30pm - 9pm UTC)
- 09/30 - 1:30pm - 4pm Eastern (5:30pm - 9pm UTC)

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

#### 09/28/2016

Today I'm going to work on ingesting another complimentary set of data.

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
