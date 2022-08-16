# bellabeat_mysql
google analytic certificate - capstone 
Bellabeat, a high-tech manufacturer of health-focused products for women. Bellabeat is a successful small company, but they have the potential to become a larger player in the global smart device market. 

## Product Portfolio
○ Bellabeat app: The Bellabeat app provides users with health data related to their activity, sleep, stress, menstrual cycle, and mindfulness habits. This data can help users better understand their current habits and make healthy decisions. The Bellabeat app connects to their line of smart wellness products.
○ Leaf: Bellabeat’s classic wellness tracker can be worn as a bracelet, necklace, or clip. The Leaf tracker connects to the Bellabeat app to track activity, sleep, and stress.
○ Time: This wellness watch combines the timeless look of a classic timepiece with smart technology to track user activity, sleep, and stress. The Time watch connects to the Bellabeat app to provide you with insights into your daily wellness.
○ Spring: This is a water bottle that tracks daily water intake using smart technology to ensure that you are appropriately hydrated throughout the day. The Spring bottle connects to the Bellabeat app to track your hydration levels.
○ Bellabeat membership: Bellabeat also offers a subscription-based membership program for users. Membership gives users 24/7 access to fully personalized guidance on nutrition, activity, sleep, health and beauty, and mindfulness based on their lifestyle and goals.

## Task:
1.analyzing smart device fitness data could help unlock new growth opportunities for the company. 
      2.gain insight into how people are already using their smart devices. 
      3.guide marketing strategy for the company.
      4.To analyze smart device usage data in order to gain insight into how consumers use non-Bellabeat smart devices. select one
         Bellabeat product to apply these insights to in your presentation.


Key stakeholder: Urška Sršen: Bellabeat’s cofounder and Chief Creative Officer
                 Sando Mur: Mathematician and Bellabeat’s cofounder; key member of the Bellabeat executive team
                 Bellabeat marketing analytics team: A team of data analysts responsible for collecting, analyzing, and
                 reporting data that helps guide Bellabeat’s marketing strategy. 
                 
Exist marketing channels: The company has invested in traditional advertising media, such as radio, out-of-home billboards, 
print, and television, but focuses on digital marketing extensively. Bellabeat invests year-round in Google Search, maintaining active 
Facebook and Instagram pages, and consistently engages consumers on Twitter.
Additionally, Bellabeat runs video ads on Youtube and display ads on the GoogleDisplay Network to support campaigns around key marketing dates.

produce a report with the following deliverables:
        1. A clear summary of the business task 
        2. A description of all data sources used
        3. Documentation of any cleaning or manipulation of data
        4. A summary of your analysis
        5. Supporting visualizations and key findings
        6. Your top high-level content recommendations based on your analysis
        
public data that explores smart device users’ daily habits.
Dataset:FitBit Fitness Tracker Data (CC0: Public Domain, dataset made available through Mobius):
Quantitive: Thirty eligible Fitbit users consented to the submission of
            personal tracker data, including minute-level output for physical activity, heart rate, and sleep monitoring. It includes
            information about daily activity, steps, and heart rate that can be used to explore users’ habits.
            
Limitation: the dataset is not clean and completed. 

Prepare
Guiding questions
● Where is your data stored? - local
● How is the data organized? Is it in long or wide format? - 
● Are there issues with bias or credibility in this data? Does your data ROCCC?
● How are you addressing licensing, privacy, security, and accessibility?
● How did you verify the data’s integrity?
● How does it help you answer your question?
● Are there any problems with the data?

Exercise Intensity - METs
MET stands for the metabolic equivalent of task. One MET is the amount of energy used while sitting quietly. Physical activities may be rated using METs to indicate their intensity. For example, reading may use about 1.3 METs while running may use 8-9 METs. METs can also be translated into light, moderate, and vigorous intensities of exercise.4

User activities in this dataset are grouped into 4 categories: sedentary, light, moderate and vigorous intensities.

MET Range	Description	Example
0 - 1.5	Sedentary	Sitting, reclining, or lying down
1.6 - 3.0	Light	Walking at a leisurely pace or standing in line at the store
3.1 - 6.0	Moderate	Walking briskly, vacuuming, or raking leaves
6.0+	Vigorous	Walking very quickly, running, taking an aerobics class, or shoveling snow
These patterns can be used to classify users. The distribution of the activities of users shows that most have a preference for moderate and vigorous activity.

There are 5 kinds data. 1. Calories, Intensity, steps. They are related. Minute dataset seems useless and they occupy much bigger space. 2.The table of heartbeat_second is not completed, only contains 14 record of 30 users. I firstly want to check if there is any user record abnormal heart beat in the dataset, which means the device might be able to be an alarm to high risk users. It's easy to cause bias so I remove it from the database. Only 8 users fill their weight in the dataset, which means quite a big part of the users are not willing to fill their weight manualy. If I use this dataset,  it could be bias too. However, weight is a tangeble metrix, I will try to use the only record and find some insight from them. To summarize, I will use daily and hourly calories, steps, and intensities, along with daily sleep， activities(including daily calories, steps and intensities), and the existing weight data to look for the insight on how consumers use non-bellabeat devices. 
1) When is the most active hour generally? Generate content for marketing. 
2) Is sedentary time related to weight loss? or is sedentary a bad habit? 
3) 24 records in the daily_sleep. Does any of activities lead to better sleep? 
4) Weight loss related to activities? 
5) How to collect weight data? 
6) The most active users and the least active users? What's their difference? 
7) Activities corelate to calories? Veryactive or overall active? 




