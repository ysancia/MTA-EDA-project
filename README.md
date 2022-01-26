

# COVID-19 and MTA Staffing

## Abstract

During the recent spike in COVID-19 cases caused by the omicron variant many industries have faced worker shortages and found themselves short-staffed. The New York City Metropolitan Transportation Authority (MTA) also felt the impact of worker shortages. The purpose of this project is to examine how usage changed for each train on the MTA due to the previous surge in COVID-19 cases in 2020 and provide initial findings about which train lines’ schedules could be adjusted to maximize limited resources. I used data provided by the [NYC MTA](http://web.mta.info/developers/turnstile.html) as well as data from the [NYC Health Department](https://github.com/nychealth/coronavirus-data). After looking at the data, I created visualizations to help communicate my findings.

## Design

I am assuming that the MTA system determines its schedules by train line rather than station-by-station (as it wouldn’t make sense to run a train to service only a couple of stations), so my analysis focused on looking at each line as a whole. 

In order to determine how MTA usage changed due to the COVID-19 surge in 2020, I looked at three time periods: December 2019 - February 2020 (pre-surge), March 2020 - May 2020 (lockdown), and June 2020 - August 2020 (reopening). 

Although the first reported case of COVID-19 in the NYC Health Department data was on February 29, 2020, I elected to begin the dataset on the following day, March 1, 2020, for ease of analysis. This should have minimal impact on the analysis as there was only one reported case prior to dates of the dataset.

## Data

The dataset from the MTA includes 8,068,861 rows of information about the location of a turnstile and how many entries and exits each turnstile had at a given date and time. These “snapshots” were taken throughout each day and indicate the amount of traffic each turnstile would experience during the three time periods.

The NYC health department data contains 184 rows of data about the cases reported by date from March 1, 2020 - Aug 31, 2020.


## Tools
- DB Browser and SQLite were used to create a database
- NumPy and Pandas were used to examine the data
- Matplotlib and Seaborn were used to create plots
