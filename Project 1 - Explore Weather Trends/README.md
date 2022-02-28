## Explore Weather Trends 
### Cities: 
* Abuja
* Kano
* Lagos

### Contents: 
* Data Extraction
* Data Exploration
* Data Visualization 
* Data Analysis 

## Data Extraction
SQL was used to extract the data from the database on Udacity classroom. Investigating the data reveals that there were a couple of missing rows for the selected cities before 1873, hence the query was written to extract data from 1873 upwards.
### First query to extract 3 cities in Nigeria
```
SELECT year, city, avg_temp
FROM city_data
WHERE year >= 1873 AND year <= 2013
AND city IN ('Abuja','Lagos','Kano');
```

### Second query to extract global data
```
select *
from global_data
where year >= 1873 and year <= 2013;
```

## Data Exploration 
For better visualization, a 7-year moving average was calculated using excel formula, below is the snippet for the analysis:

## Data Visualization 

![image](https://drive.google.com/file/d/1fNdzJ-Ksp09p-UtohxRZ7fLUxvK1_CG-/view?usp=sharing)

## Data Analysis 
1. Increasing Temperature: Analysis shows that there is a general increase in temperature, with Lagos recording the highest temperature at 27.47°C.
2. Temperature Spike: There is a downward surge in temperature between 1878 and 1895 in all the cities as well as the global dataset
3. Lagos is relatively hotter than other cities in Nigeria
4. Cities in Nigeria have higher temperatures than the global average, primarily because Nigeria is located within the tropical equator, with high temperature.

## Credits 
Sincere appreciation to Access Bank for providing this wonderful learning engagement, and to Udacity for such a content-rich experience. 