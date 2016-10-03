---
layout: page
title: About My Project
description: What project am I livestreaming?
---

### Overview

I am working on building public metrics of government services in the United
States that are available to communities across the country. I am starting with
the criminal justice system for obvious reasons.

My initial quest for data led me to the exhaustive and underutilized Uniform
Crime Report data from the FBI. A research-ready version of this data is hosted
by the [National Archive of Criminal Justice Data](https://www.icpsr.umich.edu/icpsrweb/NACJD/)
hosted by [ICPSR](https://www.icpsr.umich.edu/icpsrweb/ICPSR/).

I will be attempting to estimate expected crime rates for cities in the US and
look for community factors that influence them. There is a lot of discussion about
crime in the US, but much of it is devoid of analysis that community advocates
can use to improve their services locally. I want to fill that void.

### Roadmap

I am livestreaming different aspects of my data science work. I see the roadmap
for my work as follows:

#### Ingestion

I have completed ingesting most of the data I will need by parsing fixed width
files provided by NAJCD, applying the codebooks to the data, and then loading
the data into a SQL database.

#### Cleaning

I am currently working on cleaning the data. The way I am approaching this is
to write a series of functions that I can apply to the raw data upon extraction
to clean up different types of data issues for different analyses. I am in the
process of mapping out these different types of data issues, writing the functions,
testing them, and then improving them for performance.

#### Exploratory Analysis

Cleaning and exploratory data analysis go hand in hand. While cleaning I plan to
start documenting the relationships among various elements of the data to
understand the linkages in the data and to identify possible areas for improvement
by enforcing business rules to deal with various issues in the data (e.g.
  negative counts).

#### Joining Additional Data

After I have wrangled the main dataset (UCR crime reports) I plan on joining
contextual data to help me understand the patterns in crime reporting.

#### Modeling

This is the final step. 
