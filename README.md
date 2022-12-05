# Food-Establishment-Inspection-Scores-Analysis

Food Establishment Inspection Scores Analysis
[I320D – Fall 2022]
Sreeja Ambati,
Audrey Dahlkemper,
Zachary Eagan,
Xavier Hernandez,
Pranutha Punukula


1 Problem Introduction
_______________________

We are interested in seeing if restaurants who receive a low score will either increase their inspection score, be removed from the data set (go out of business), or change their location (zip code) the following year. We will analyze the dataset to identify the overall trends of the various inspection scores of different restaurants. First, we will determine a threshold for what appears to be a concerningly low inspection score, then we will analyze the score change or removal trends of the low score restaurants in the following years. The data will be plotted to visualize these trends and see if scores are increasing or decreasing over time. By analyzing how different restaurants respond to receiving a low inspection score, we will learn how scores affect the behavior of an establishment and/or its customers. The statistical findings, combined with additional information about the restaurants can create a better understanding of what timeline low scoring restaurants fall into, indicate potential trends in restaurant types, and what effective business strategies restaurants can take to mitigate these issues.

2 Dataset
__________

The Food Establishment Scores data set tracks the inspection scores of restaurants in the Austin area from 2019 to 2022. Inspections are conducted in accordance with the Texas Food Establishment Rules (TFER) and City of Austin Codes for the City of Austin Department of Austin Public Health. Inspections are completed by Environmental Health Officers working for Austin Public Health (APH) Environmental Health Services Division (EHSD). Included variables are restaurant name, zip code, inspection date, score, address, facility id, and process description. 25,842 different examinations have been recorded. 

Each grain of data represents an individual inspection of a restaurant on a specific date. The attributes include the restaurant name and facility ID, location, inspection date, and inspection score. 


3 Models and Techniques
_______________________

We will analyze the data to see the overall trends of various inspection scores of different restaurants. First, we will determine a threshold for what appears to be a concerningly low inspection score, then we will analyze the score change or removal trends of the low score restaurants in the following years. The data will be plotted to visualize these trends and see if scores are increasing or decreasing over time.

In Texas, a food establishment inspection score can fall within the following ranges - Excellent: 100 to 97, Good: 96 to 90, Satisfactory: 89 to 81, Poor: 80 to 71, Failing: 70 or below. A "low" inspection grade is anything below a 70. The standard procedure for a store that receives a score below 70 is an issuance of fines, a follow-up inspection, and in certain cases closure of the restaurant. If a follow-up inspection is ordered it is scheduled 3-10 days after the annual inspection in order to see if the owners made corrective actions. Over the past three years 402 establishments received a score below 70 but only 317 received a follow up inspection. This could allude to a potential 85 stores going out of business. 

In order to analyze the difference in initial inspection scores and the follow up inspection scores a new data frame was created. The data frame used for analysis includes the variables restaurant name, zip code, addresses, first inspection date, first inspection score, follow-up inspection date, and follow-up inspection score. Each line was filtered first through the low score function and then the follow up inspection function. As after an establishment receives a grade below 70 they also receive a follow up inspection. The variable "first inspection date" refers to the annual inspection while the variable "follow up inspection date" refers to the first follow up inspection after the annual.

We then imported the statistics package in order to plot as a histogram the difference between the follow up inspection score and the first inspection score calculated in order to analyze the change over time. 

4 Results and Discussion
_________________________

An analysis of the restaurants with the ten lowest scores exemplifies a correlation between a store receiving a low score and then a follow-up inspection. Out of the ten establishments, 2 received a low store and did not record a follow up inspection. Cross tabulating the dates of the two stores - Dr. Wok and Mom's Taste - it appears that given the date each store closed. The time period between routine inspections and follow up inspections is often a couple or days and at most a month. Dr. Wok and Mom's Taste recorded no follow up inspection within that range. The other restaurants who received a low score during a routine inspection increased the score during the follow up inspection. 

<img width="521" alt="Screen Shot 2022-12-05 at 3 53 06 PM" src="https://user-images.githubusercontent.com/51467244/205750253-f280b380-96e4-47d1-aab9-7c309f447e43.png">

The histogram above displays a left-skewed unimodal distribution of the filtered restaurant inspection scores. On the histogram the mean is represented by the black dashed line. The mean is 17.49 which in regards to the data set is interpreted as an average increase of 17.39 points between the initial and follow up inspection. The variance is 84.84 and the standard deviation is 9.21. 

5 Conclusion
_____________

Before conducting the analysis, we anticipated that restaurants who received a low score would either increase their inspection score, be removed from the data set due to going out of business, or change their location the following year. We believed that receiving a threshold-met low score would challenge the restaurant’s current management practices, and force them to either take drastic changes to improve their score or shut down. We predicted that some confounding variables could be that the data points were from the past few years including the quarantine period for COVID-19 which generally negatively impacted many businesses and the many restaurant shut downs in popular areas in Austin due to increased rent from the influx of new people in Austin. The analysis tool we selected was conducting a statistical analysis on the restaurants that fell under the low threshold score. We ran a correlation test of the restaurants with the ten lowest scores between a store receiving a low score and then a follow-up inspection. We believed this was the most effective way to determine the overall trends of various inspection scores of different restaurants. 

We learned that restaurants that received a low score during their initial inspection either shut down between the period that they had their initial and follow-up inspection or managed to increase their score by an average of 17.39 points. This implies that the time between the initial and follow-up inspection is a critical determinant period for the fate of the restaurants. Receiving a low score means that the restaurant has to either drastically change their management practices to comply with the Texas Food Establishment Rules (TFER) and City of Austin Codes for the City of Austin Department of Austin Public Health, and if not done they will likely be forced to shut down. 

Our findings may be generalizable to grocery stores, bars, mobile vendors, food manufacturers, food warehouses, coffee bars, bakeries, convenience stores, and some child care centers in Austin. This is because all of these establishments also require semi-annual inspections following both Texas Food Establishment Rules (TFER) and City of Austin Codes for the City of Austin Department of Austin Public Health. These findings may also uncover information about restaurants in Texas in general because the inspections are conducted in accordance with the Texas Food Establishment Rules. However, it is unlikely that it would be as accurate because the inspection also accounts for Austin specific food health requirements which may be stricter or more lenient in certain areas. 

Our proposed solution is to ensure that thorough inspections are done when the restaurant has opened to make sure they are complying to both Texas Food Establishment Rules (TFER) and City of Austin Codes for the City of Austin Department of Austin Public Health. Restaurant owners and managers should also fill out a form initially to make sure they have a solid plan to meet the inspection requirements. Enforcing these rules in the beginning will prevent restaurants having to scramble at the last minute to make sure they are receiving good inspection scores. Restaurant owners and managers will be more aware of the rules and regulations from the beginning and be able to implement better practices without having to learn the stressful way. Restaurants that still don’t meet expectations will have the same period of time to improve their scores or shut down. This solution is fair because it allows restaurant managers and owners to be more aware of how they should be running a restaurant from the beginning and allows for an omission of the potential fines received for low scoring restaurants that violate certain restrictions. This allows the restaurant management to plan and implement practices more effectively to ensure they are starting from a baseline of meeting the rules and regulations. If restaurants still don’t meet these rules and regulations after giving clear expectations initially, then action will be taken accordingly to make sure they meet these expectations or shut down. Since inspections are not set to happen at any specific or predictable date, improving scores on a strict timeline may be easier or more difficult due to external economic factors, and better prevented if these rules are strictly enforced in the beginning.  

6 References
_____________

- https://data.austintexas.gov/Health-and-Community-Services/Food-Establishment-Inspection-Scores/ecmv-9xxi

- https://www.austintexas.gov/department/food-protection



