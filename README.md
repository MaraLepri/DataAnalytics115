# DataAnalytics115

For this class, I have copied some data from the Department of Housing and Urban Development: 
https://www.huduser.gov/portal/datasets/ahar/2020-ahar-part-1-pit-estimates-of-homelessness-in-the-us.html

This data was very, very clean when it was posted on the HUD website. I did not run into problems with duplicate entries or missing data or entries that didn't make sense. The only thing I did was remove some of the colums to make the data easier to look at for myself. There were several columns on the original dividing entries by age groups per ethnic group, by veteran status, etc, that I did not copy into my data here.

Here are the columns I did keep:

 [1] "CoC Number"                                                        
 [2] "CoC Name"                                                          
 [3] "Overall Homeless, 2020"                                            
 [4] "Overall Homeless - Under 18, 2020"                                 
 [5] "Overall Homeless - Age 18 to 24, 2020"                             
 [6] "Overall Homeless - Over 24, 2020"                                  
 [7] "Overall Homeless - Female, 2020"                                   
 [8] "Overall Homeless - Male, 2020"                                     
 [9] "Overall Homeless - Transgender, 2020"                              
[10] "Overall Homeless - Gender Non-Conforming, 2020"                    
[11] "Overall Homeless - Non-Hispanic/Non-Latino, 2020"                  
[12] "Overall Homeless - Hispanic/Latino, 2020"                          
[13] "Overall Homeless - White, 2020"                                    
[14] "Overall Homeless - Black or African American, 2020"                
[15] "Overall Homeless - Asian, 2020"                                    
[16] "Overall Homeless - American Indian or Alaska Native, 2020"         
[17] "Overall Homeless - Native Hawaiian or Other Pacific Islander, 2020"
[18] "Overall Homeless - Multiple Races, 2020"                           
[19] "Sheltered Total Homeless, 2020"                                    
[20] "Unsheltered Homeless, 2020"                                        
[21] "Overall Homeless Individuals, 2020"                                
[22] "Overall Homeless People in Families, 2020"                         
[23] "Overall Chronically Homeless, 2020"                                
[24] "Sheltered Total Chronically Homeless, 2020"                        
[25] "Unsheltered Chronically Homeless, 2020"                            
[26] "Overall Homeless Veterans, 2020"   

I created a scatterplot which reveals that there is a relationship between the number of males, females, non-chronically homeless. It's fairly straightforward: with this positive relationship, if there is a high number of any one of these categories, the other categories are likely to also have a higher number. These are strong correlations, greater than 0.90 for all categories. 

To do this, I just ran ggpairs on the data:

> ggpairs(Homeless2, title="Scatterplot of Genders, Chronicity and Shelter status of Homeless Peoples")

For non-binary folks, they were only somewhat related to chronically homeless people and unsheltered people, with correlations of about 0.70. The relationship drops off from there, from 0.60 down to 0.40 prediciton of increased numbers in other categories. 

Here is that visual, and it's in my repository as well. The last two tabs say Chronically Sheltered and then Chronically Unsheltered. Apologies for the formatting there. I will try to fix it when I have some free time. 

![scatterplot](https://user-images.githubusercontent.com/92341860/144087583-11e727e9-820f-4757-b327-87f1456f6f9a.png)


Thanks for checking out my very beginner page!
