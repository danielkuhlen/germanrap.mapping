# Introduction

This data project provides interactive maps and data on the success of different states and districts in Germany's rap industry. The project aims to answer the question of which city produces the most successful German rappers, and therefore, which city is the most important in this industry. The data provided can also be used to analyze general questions regarding the origins of German rappers.

# Publication

This project, coding documentation and the interactive maps are published in a bookdown format, available at the following URL:

https://danielkuhlen.github.io/germanrap.mapping/

The bookdown format allows for a more comprehensive and interactive presentation of the data and results, making it easier to understand and explore the findings. 

# Data

The *germanrap.origin* dataset contains information on various music projects, including the artist/group name, type of project, number of weeks at number one, and city, district, and state of origin. This dataset can be accessed using the following URL:

https://raw.githubusercontent.com/danielkuhlen/germanrap.mapping/master/germanrapper.origin.csv 

In detail these variables are included in the dataset:

| Variable Name        | Description |
|----------------------|-------------|
| id                   | A unique identifier for the project |
| artist.name          | The name of the artist or group associated with the project |
| project.name         | The name of the project |
| weeks.nr1            | The number of weeks the project was at number one on a chart |
| number.collaborators | The number of collaborators involved in the project |
| weeks.nr1.adj        | The adjusted number of weeks the project was at number one |
| award                | The award received by the project |
| type                 | The type of project, such as an album or single |
| city.origin          | The city of origin for the artist or group |
| kreis.origin         | The district of origin for the artist or group |
| state.origin         | The state of origin for the artist or group |
| running.number       | A sequential number assigned to each project in the dataset |

## Downloading the Data in R

To download the dataset in R, you can use the `read.csv` function from the base R library.

Here is an example of how to use the `read.csv` function to download the data:

```
germanrap.origins <- read.csv("https://raw.githubusercontent.com/danielkuhlen/germanrap.mapping/master/germanrapper.origin.csv")
```

## Downloading the Data in Python

In Python, you can use the `pandas` library to download and read the csv file. To do this, you can use the `read_csv` function from the `pandas` library.

Here is an example of how to use the `read_csv` function to download the data in Python:

```
import pandas as pd

germanrap.origins = pd.read_csv("https://raw.githubusercontent.com/danielkuhlen/germanrap.mapping/master/germanrapper.origin.csv")
```

## Downloading the Data in Stata

In Stata, you can use the `import delimited` command to download and read the csv file. 
Here is an example of how to use the `import delimited` command to download the data in Stata:

```stata
import delimited "https://raw.githubusercontent.com/danielkuhlen/germanrap.mapping/master/germanrapper.origin.csv", clear
```

# Citation

If you use this repository or its contents in your work, please cite it as follows:

Kuhlen, Daniel. (2023). germanrap.mapping: Mapping rap success for states and districts in germany. GitHub repository: https://github.com/danielkuhlen/germanrap.mapping
