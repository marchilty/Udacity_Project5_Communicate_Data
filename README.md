
# Chronic illness: symptoms, treatments and triggers

## Introduction
**This project is part of Udacity's Data Analyst Nanodegree Programm. <br> The dataset was aquired from kaggle.com (https://www.kaggle.com/flaredown/flaredown-autoimmune-symptom-tracker). The website Flaredown tracks chronic illness symptoms and provided the data I use in this project. And has more than 3 million rows that would not be usable using non programmatic approaches. Sources are marked with (n) and linked under Sources at the end of the notebook.**

#### About the data (from Flaredown)

Instead of coupling symptoms to a particular illness, Flaredown asks users to create their unique set of conditions, symptoms and treatments (“trackables”). They can then “check-in” each day and record the severity of symptoms and conditions, the doses of treatments, and “tag” the day with any unexpected environmental factors.

**User**: includes an ID, age, sex, and country.

**Condition**: an illness or diagnosis, for example Rheumatoid Arthritis, rated on a scale of 0 (not active) to 4 (extremely active).

**Symptom**: self-explanatory, also rated on a 0–4 scale.

**Treatment**: anything a patient uses to improve their symptoms, along with an optional dose, which is a string that describes how much they took during the day. For instance “3 x 5mg”.

**Tag**: a string representing an environmental factor that does not occur every day, for example “ate dairy” or “rainy day”.

**Food**: food items were seeded from the publicly-available USDA food database. Users have also added many food items manually.

**Weather**: weather is pulled automatically for the user's postal code from the Dark Sky API. Weather parameters include a description, precipitation intensity, humidity, pressure, and min/max temperatures for the day.

If users do not see a symptom, treatment, tag, or food in our database (for instance “Abdominal Pain” as a symptom) they may add it by simply naming it. This means that the data requires some cleaning, but it is patient-centered and indicates their primary concerns.

## Summary of Findings

This dataset is really hard to work with, because all information is scattered between dates and different topics for each user. In case of this dataset visual representation is often not my prefered method of analyzing, I would prefer tables in most cases. Since this project should focus on visuals only I will do my best to include as much information as possible within them.
Nevertheless the dataset showed interesting characteristics of patients suffering from chronic illness. First of there are mainly women under the age of 60 using the app regularly. We can tell that most chronic illness patient in this group suffer from fibromyalgia, depression and anxiety. The most common symptoms include fatigue, headache and nausea which fits most diseases well. Ibuprofen is by far the most used drug for all patients in the dataset. Bivariate analysis showed no correlation between disease activity and age. Neither did the pain scale correlate with age. Overall there seems to be a tendency for higher pain values during winter months compared to the rest of the year (~.5 difference in pain on a scale from 0-4). I tried focusing on one condition, in this case fibromyalgia, but at the moment I cannot find the time to further explore it. This will probably added later. 

Epidemiological studies have shown that in most cases progressing age is associated with higher disease activity.  


## Key Insights for Presentation

The key feature of this dataset is the large amount of information for a heterogenetic disease spectrum. I want to represent most of the strengths of the dataset in my presentation. This means focusing on epidemiologic data and leaving out detailed analysis of specific forms. I cannot guarantee that the data is standardized enough to allow assumptions in smaller groups. 

First of we will look at the general features of the dataset that are important for conclusions. This mean looking at age and gender distributions as well as the underlying diseases. I use barplots and histogramms.

From there we move on to see how age is correlating with the diseases. I use a heatmap to compare categorical data with age. After that a lineplot shows how the disease activity changes over years. 


