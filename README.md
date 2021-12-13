# ak4656 and bs3366 | Group Project | tools for analytics

Class: 
Tools for Analytics Fall 2021

Section: 
01

Instructor: 
Julian Berman 

CREATORS/STUDENTS: 
Alexis Kim (ak4656)
Eldine Sam (bs3366)

Group name: 
Group 55

Project: 
Final Group (55) Project for the class

Description: 
This repo possesses two files that analyzes local NYC 311 data from 2020:  
1. Top10.ipynb: 
    Here we have a jupyter notebook that surveys the 2020 311 NYC data and displays the top 10 incident type from descending prevalence. They are labeled by incident type and contained to a specific zipcode. We hard coded the zipcode to be 10027. 
    
    Implementation: 
        a. We created a pandas dataframe and filtered the dataframe according to the zipcode of our choice, 10027. 
        b. We then created a series of our dataframe specific to our zipcode according to complaint type and then counted the number of incidents.
        c. The series was already sorted by descending prevalence and so the top 10 incident types were then filtered for and presented. 
    
2. Parking.ipynb: 
    This jupyter notebook compares the parking incident within all of NYC to the parking incident in one specified zipcode in the city. The comparison is generated as a ratio and then the ratio was used to calcuate a boolean value of greater than or less than for comparison of NYC to a specified zipcode. 

    Implementation: 
        a. We created a dataframe of the 311 calls in NYC in 2020 and filtered the complaint types to only incident types of "Illegal Parking" for the whole city. We then counted the number of rows within this filtered dataframe in order to get the number of incidents. 
        b. We then calculated the number of incidents for the whole city using the aforementioned method above. With these two values, we took the ratio of illegal parking in NYC : total incidents in the city 
        c. We then repeated steps a. and b. above but instead we confined the area to our specified zipcode of 10027. For this proprotion we calculated the ratio of illegal parking in zipcode 10027 : total incidents in 10027
        d. We compared the ratio of the zipcode illegal parking infractions to the citywide illegal parking infraction ratio. We used a boolean value to compare the two ratios. 
