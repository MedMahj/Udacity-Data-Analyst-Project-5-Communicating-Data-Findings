# Udacity Data Analyst Project 5 - Communicating Data Findings


## Dataset (Ford GoBike System Data)

> This dataset includes information about individual rides made in a bike-sharing system covering the greater San Francisco Bay area. The data consisted of ride duration and attributes of appoximately 180,000 individual rides. The attributes included information about ride time and stations, as well as additional information about users such as type, gender, birth year. Some data points were removed from the analysis due to inconsistencies or missing information. New features were added like start_day_week, start_hour, member_age, age_groups .

> In this investigation of the Ford GoBike System, I wanted to look at trip distribution and the most common user behaviors and characteristics, specifically how user type, time, gender, and age impacts usage of the system.

## Project Requirement:

> we will need an installation of Python, plus the following libraries::

* pandas
* NumPy
* Matplotlib
* seaborn

## The files included are:
```sh
* exploration.ipynb : jupyter notebook for data exploration
* exploration.html : html file for data exploration
* 201902-fordgobike-tripdata.csv : csv file contains dataset
* slide_deck.ipynb : jupyter notebook for  explanatory analysis
* slide_deck.slides.html : slide deck presentation of explanatory analysis in HTML format
* output_toggle.tpl : templete used to hide code cells from nbconvert
```

## How to view Slide Deck

> Use the following expression on the command line to open up the slide deck for viewing :

```sh
jupyter nbconvert slide_deck.ipynb --to slides --no-input --no-prompt  --post serve
```

## Summary of Findings

**Distribution of Rides by User Type, Gender,Age and Time**
- Subscribers contributed the majority of the bike usage, about 90%, while about 10% were consumed by cusomters (or casual users)
- Most riders were male.
- The number of rides depends on user age. The bar plots below shows a huge usage of the bike share system by young adults (25-34 years old) espacially 31 years old riders.
- The trip distribution over day hours peaks around two timeframes, 7am-10am and 16pm-19pm, during typical rush hours. 
- Looking in combined with the trip distribution over day of week plot, it is quite obvious that the majority of rides happened on work days (Mon-Fri).

**Distribution of Ride Durations**
- Duration has a long-tailed distribution, with a lot of rides on the low duration end, and few on the high duration end. the proportion of outliers is 5.33%, that means 94.67% of rides were less than 1488s
- When plotted on a log-scale, the duration distribution looks like normal distribution, with one peak aroud 500s. we could reduce the proportion of outliers to 1.5%.
- Subscriber ride duration is smaller than Customer and male riders tend to have shorter trips compared to female users. 
- Young male subcribers are the fastest riders and female senior customers are the slowest.
- Ride duration average is smaller and more stable duraing the rush hours
- The average usage time shown an increasing trend during normal hours

## Authors

* **Mohamed BOUSETTA MAHJOUB** - *Initial work* - [MedMahj](https://github.com/MedMahj/)
