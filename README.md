# Air Quality Throughout the Years 1980-2021 

## Motivation 
I decided to do my research on the air quality because I did my english paper on air pollution and I have always had interest on air quality. Plus it is one of the most of the important source needed to keep humans and other living creatures alive. With a lot of talk about how we have to become more sustainable I wondered how the air quality has changed since we implented Clean Air Act and other Acts to improve air quality. Are they working or are they not that effective?

## Data Source 
The data was made by the EPA where they took the measure of AQI of Counties in the United States of America. They also look at the number of days where aqi was 0-50 which is good, 51-100 which is moderate, 101-150 which is unhealthy for sensitive groups, 151-200 which is unhealthy, and 201 and above is very unhealthy, and hazardous which rarely happens. There is measure of the highest aqi recorded that year, median aqi, and pollutants that were the main cause of the pollution. 

## Processing Steps 
Since the data was all seperated by year I had to merge all of the data into one csv file so I will be able to work on it. So, I used R to make dataset of all of the csv files. After putting it into one file I saw that not every County had aqi data for every day and there missing data for a few of the counties for some years. So I decided to choose one county that all of the data and was known for not having good air quality. So, I chose Los Angeles county that was known for not having bad air quality. In R I made a new dataset by only taking the rows that had Los Angeles in them, I could easly use the data. 

## Visualization 
![image](https://user-images.githubusercontent.com/91635769/144725984-774ff70c-ed21-4ad8-9c01-1848debdf715.png)

It is a bar graph of the yearly median aqi of Los Angeles. It starts at 150 which is not the ideal aqi but as it we get to 1995 the aqi starts to drop 100 and below. There was the most change between 1989 and 1990. 

![image](https://user-images.githubusercontent.com/91635769/144726419-443e1abd-308a-412b-9f70-c3ce7ae6a737.png) 

The highest max aqi seems the same for every except 1980 and 1991.

![image](https://user-images.githubusercontent.com/91635769/144726434-b550a0ed-c97d-4544-b0fd-8635c511acae.png) 

The max aqi outliers is explained in the hazordous days becuase the only hazordous days were in 1980 and 1991 which whill explain why the max aqi that year was higher than all of the other years. 

![image](https://user-images.githubusercontent.com/91635769/144726440-bccc8622-e128-4d8e-90d1-a53c4fd3bb79.png) 

The amount of very unhealthy days drastically decreases from 1980 to 1996. 

![image](https://user-images.githubusercontent.com/91635769/144726444-4fe41c0c-3c5a-48e5-9e71-c7c774dc062b.png)

The amount of unhealty days seem to go up and down.

![image](https://user-images.githubusercontent.com/91635769/144726450-5ed3ba0c-35e7-413c-a43f-62059b5a000f.png) 

The amount of unhealthy days for sensitive groups seems to be the same for every year except for 2021 probably because they didn't get all of the data from 2021 yet.

![image](https://user-images.githubusercontent.com/91635769/144726452-73f9ec8c-2e9b-4b79-b753-3e13d51deae3.png)

The amount of moderate days seems to have gone up probably because in the 1980s there were more hazordous days but now there is less hazordous days and more moderate days.

![image](https://user-images.githubusercontent.com/91635769/144726454-af06d2ab-4d66-4e02-9b4a-298d9102d8bd.png)

The amount of good days seems to go up and down but the amount of good days compared to the 1980s has gone up. 

## Analysis 

For analyzing my data I used the boxplot to find out the variance between my data and to see if there are any significant outliers. 

<img src = https://user-images.githubusercontent.com/91635769/144728519-3999f6c5-99ab-431c-ab5a-62336d04ee10.png width= 50%, height = 50%> 

For good days there are some outliers on the top which are probably from the spikes that is found in the bar graph. But I think it is needed in the data because it is big factor on the median aqi. 

<img src = https://user-images.githubusercontent.com/91635769/144728605-e79c4cf8-7395-40bc-a394-3b2f64a320ac.png width = 50%, height = 50%> 

The moderate days seems to be skewed a little bit to the left as there are more days in a year with moderate days. Which is seen by the increase in moderate days from 1980 to 2021.

<img src = https://user-images.githubusercontent.com/91635769/144728623-113dc598-2bab-4785-a1a6-3b1607196139.png width = 50%, height = 50%> 

The unhealthy for sensitive boxplot seems to have 1 outlier at the bottom and 1 outlier on the top 

<img src = https://user-images.githubusercontent.com/91635769/144728638-3300c0c6-1c8f-4277-9c07-7291cebb87c4.png width = 50%, height = 50%> 

The boxplot for unhealthy seems to be left skewed as the median is closer to the top. 

<img src = https://user-images.githubusercontent.com/91635769/144728653-53e71f04-2e5b-484c-8185-e43a6ae74e23.png width = 50%, height = 50%> 

The very unhealthy days median is closer to the bottom as seen in the bar graph the amount of very unhealthy days has drastically so the median is closer to the bottom than the top. It is skewed down 

<img src = https://user-images.githubusercontent.com/91635769/144728672-bba73ee6-5276-4bf0-b9ce-d92ebdf8dfd5.png width = 50%, height = 50%> 

There is going to be outliers for hazardous days becuase there were only 2 days throughout 1980-2021 in Los Angeles that were recorded as hazardous days. Which found from the max aqi outlier. 

<img src = https://user-images.githubusercontent.com/91635769/144728682-7076c83b-6feb-4d57-b78e-c63f32411988.png width = 50%, height = 50%> 

Max AQI boxplot seems to be skewed to the right because of the outlier at the top which is from the year 1991 where there was hazardous day that was recorded. 

<img src = https://user-images.githubusercontent.com/91635769/144728693-d37d9748-4c30-446e-a95b-9f85dbd73d8f.png width = 50%, height = 50%> 

The boxplot for the median aqi is skewed to the right as there are more days that are lower than an aqi of 100. 


The analysis helped me find out that throughout 1980 - 2021 the air quality in Los Angeles has been improving. The number very unhealthy days have gone done significally from 1980-2021 and median aqi has also gone down significally. This shows that going to more renewable resources does have affect in improving air quality. Although it will hard to predict the air quality with just the median aqi and etc but this does show that the air qualtiy has gotten better since the implementation of the Clean Air Act. 




## Description of the Code and Materials

The data came from the EPA and .csv files can be found in the aqi folder. 

United States Environmental Protection Agency. Air Quality System avaliable at https://aqs.epa.gov/aqsweb/airdata/download_files.html#Annual accessed 12, 04, 2021

