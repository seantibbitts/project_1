# project_1

1. Images
2. Using Data -- Sean E's CSVs
3. Investigating Solar Power PowerPoint -- Presentation slides
4. Investigating Solar Power Word Doc -- Write-up
5. Project 1 Draft -- Sean T's IPython Notebook
6. Project1 -- Ahmad's IPython Notebook
7. Solar PV consumption by country -- Sean E's 1st IPython Notebook
8. Solar PV energy consumption by region -- Sean E's 2nd IPython Notebook

## Introduction
We were interested in the state of solar power in the United States and globally, and the relationship between solar power and unemployment.

## Q. Where Could Solar Power Help Unemployment?
We gathered data from the U.S. Census using the Census package in Python, and downloaded the rest of the data from various government websites, including The Open PV Project, CDC/NLDAS and the U.S. Energy Information Administration.
Our goal was to map unemployment and sunniness data against solar installs and utilities to find areas of the U.S. where both measures are high but where solar power use is low.

The gmaps package struggles to plot more than 1,000 points at once (trying crashes the entire Jupyter Notebook instance), so we needed a way to distill the solar installs (1,000,000+) and the solar utilities (2,000+) down to manageable sizes. We investigated a few options, including binning latitude and longitude, and we selected k-means clustering because we wanted to keep the organic feel of the data.

We also needed a way to plot sunniness and unemployment on the same map, and we decided to use the harmonic mean of the two due to its ability to combine rates with different denominators.

We generated various plots while investigating this question, which you can find in the Images folder. The last two maps illustrate the the potential answer to our question: there are large swaths of the United States where both unemployment and sunniness are relatively high, but where there are no solar installs or solar utilities. Our conclusion: if the government (federal, state or local) invested in solar power, this could help with the unemployment levels in these areas.

## Q. How much energy is consumed by US?
Looking at the data sets via EIA, our goal was to come up with a visual that describes the percent change of the energy consumed by the U.S over time. Over the course of 60+ years, petroleum and coal consumption has decreased around the time solar and wind increase (2005-2015). Coal has been steady and has not seen any major changes over the past 60+ years. The past 30 years, wind energy consumption has dramatically gone up ~%120 between 2005-2015. Solar energy consumption is on the rise, around the same time wind energy has. Unemployment regions could play a role in helping solar energy consumption rise. 

## Q. How much solar PV energy is consumed by region and country?
We looked at Solar PV energy consumption by region as a percentage and consumption by country. We wanted to see what part of the world consumed the most solar energy as a percentage. Europe and Asian consumed the most solar energy making up more than half of the solar energy consumed by the world per year compared to South America, Africa and the Middle East that combined for 3% at the bottom. China and the United States consume the most solar energy individually, with China passing the United States. We wanted to show how other nations are pushing to expand the use of solar energy. China consumed over 60 terawatt-hours per year on the average compared to 55 terawatt-hours per year for the United States.
