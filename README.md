# BIGDATA-510AAU23 Final Project Proposal #

## The names of your team members ##
- Morgan Bratt (solo)
  - mb171@uw.edu

## The data set you plan to study and its estimated size ##
- I will be using [gwa-bitbrains](https://www.kaggle.com/datasets/gauravdhamane/gwa-bitbrains) This dataset contains performance metrics for 1250 VMs from a data-center.
- It is composed of 1250 csv files that will need to be ingested.  Each CSV file should contain performance metrics for a VM from a hosting service in the Netherlands.
- The total uncompressed size of the 1250 CSV files is 1.2 GB  

- A sample of the files in the dataset.

    [![files.png](https://i.postimg.cc/7hFtvRJK/files.png)](https://postimg.cc/BPCBHMgF)

- 111 Outliers that have incomplete time series (That I have found, there may be more as I explore the data.)

    [![outliers.png](https://i.postimg.cc/GhtwYBCQ/outliers.png)](https://postimg.cc/MXCFJpXM)

- Example data from one of the CSV files showing performance data for a VM

    [![example.png](https://i.postimg.cc/DZtW3VnJ/example.png)](https://postimg.cc/sQ4f5NBs)

## Which parts of the Spark ecosystem, or any other tools, you anticipate using to study it ## 
- I want to use spark to load in and group the data.  Once the data is formatted and aggregated I may use some data science workflows from DATASCI-530A to derive some visualizations
- This may involve translating the data from spark dataframes to pandas or handling that handoff, I have not ever done that before.

## Questions and areas of exploration you plan to undertake ##
- I want to format the data for time series analysis to understand when machines go outside certain performance thresholds and result in a business impact.
- I am looking into grouping data into percentiles per sequences (maybe hourly or 15).
- My hope as I have just started a role in Site Reliability Engineering, I can use this to exercise to learn techniques I can use on the job.
- The Kaggle description calls out that some or all of workloads running on these VMs are related to financial transactions that have closing periods with increased usage.
  - Hopefully I can illustrate these events in the data analysis.

***
***
***

# Presentation #
My goal is to present using the notebooks themselves, documented through markdown cells.  The following sections are available in offline copy below:

[1) Data Prep](https://morganbratt.github.io/BIGDATA-510AAu23__ClassProject/Data%20Prep.html)  
[2) Data Exploration](https://morganbratt.github.io/BIGDATA-510AAu23__ClassProject/Data%20Exploration.html)  
[3) Time Series Analysis](https://morganbratt.github.io/BIGDATA-510AAu23__ClassProject/Time%20Series%20Analysis.html)   
[4) Peformance Footprint](https://morganbratt.github.io/BIGDATA-510AAu23__ClassProject/Next%20Steps.html)  
[5) Next Steps]()
