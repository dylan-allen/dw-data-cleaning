# Domestic Worker Mapping Project: Survey Data Cleaning
*As part of SOC 116AC: "Work, Justice & the Labor Movement" and the UC Berkeley Labor Center*

These notebooks are written to clean data collected from California domestic workers on their demographics, commutes, and experiences with worker's rights violations. 

The survey was conducted via Google Forms and included over 400 employee responses on over 500 of their employers. Many questions asked are free response questions, or include an "Other" free response option. The data was originally collected in English, Spanish, and Mandarin, and has been translated to English (except for some free response).

## Phase 1

Originally, multiple choice questions were formatted by Google Forms as concattenated lists. These were cleaned to be formatted as True/False columns for each option. 

Many domestic workers have multiple employers. In the survey, respondents were asked to provide data on their each of their employers, and were asked a series of identical questions for each employer. Google Forms made a new set of columns for each employer response, leading the original table to have 416 (aka too many) columns. To fix this, the data was collapsed to employer level. Each employer response is a new column, and given an ascending employer ID up to the number of employers a respondent recorded. 

ZIP code and city name responses were also cleaned, and test responses were dropped.

## Phase 2

Because this project has a focus on mapping, and ZIP code responses were rare for employer locations, city names were more thoroughly cleaned.

The multiple choice question, "Employer Health And Safety Precautions", was translated into a series of True/False columns for each option.

"Other" data was categorized when possible (Number of Years Worked, Years in U.S., etc.).