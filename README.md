# Analysis of Covid Impact on Airport Traffic

![Google Colab](data:image/png;base64,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) 
![Kaggle](data:image/png;base64,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)

## Data Visualisation Project
- Geographical Plot
- Bar Graph

## Features

- Shows baseline bar graph of Countries
- Shows baseline bar graph of Cities
- Shows baseline bar graph of States
- Shows baseline bar graph of Airports
- Shows baseline Geographical Plot 

The main motive behind making this project was
> To asses the total difference between airtaffic
> from July 2020 to December 2020.
> It will help to understand how covid arrival impacted
> Airtraffic and air transportation in general

## Tech

All the tech-stack used in this project is listed below:

- [Python](https://www.python.org/) - commonly used language for data science and visulation!
- [Google Colab](https://research.google.com/colaboratory/) - a cloud based notebook style compiler.
- [Kaggle](https://www.kaggle.com/) - a huge amount dataset provider.

## Dataset

This dataset shows traffic to and from the Airport as a Percentage of the Traffic volume during the baseline period. The baseline period used for computing this metric is from 1st Feb to 15th March 2020. The dataset gets updated monthly.

This data is publicly available from [Geotab](geotab.com).
## Installation

Google colab support installation of almost all Python Library.

Install the essesntial packages like numpy and pandas

```sh
pip install numpy
pip install pandas
```

Install Kaggle

```sh
!pip install kaggle
```

## Import Dataset

Kaggle requires special auth key to communicate with its dataset. To further know how to
tranfer data from Kaggle to Google colab. PLease refer to the wonderful article written by
Kaustubh Gupta.
[Article Here](https://www.analyticsvidhya.com/blog/2021/06/how-to-load-kaggle-datasets-directly-into-google-colab/)

