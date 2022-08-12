# work-life-balance-and-achievement-data-analysis
# What can data say about work-life balance and achievement?

## Introduction
Why is work-life balance important? Every day thousands of Americans struggle with obtaining work-life balance. A healthy work-life balance is essential for many reasons. A heavy workload and excessive working hours can shift the work-life balance and make it difficult for employees to take care of their health, personal life, and family and keep their marriages, social needs, and relationships afloat. Also, stress resulting from poor work-life balance can lead to burnout and health problems, including serious chronic diseases. Good work-life balance improves our health and wellbeing, increases productivity, lowers daily stress, and gives us time to focus on what we love.

What is work-life balance? Work-life balance is something that all people try to achieve. Work-life balance is when employees will not let work run their lives. So, employees can devote specific amounts of time to their work and personal lives. Work-life balance lets us achieve personal goals while still staying productive and successful at work. According to Statista, 72% of Americans looking for a job believe that work-life balance is an essential factor to consider. (5) Many job seekers consider work-life balance when choosing a job, and companies prioritize how they effectively help their employees manage work hours.

## Project description
This project is aimed at analyzing "work-life balance" and "achievement" features of the Kaggle dataset "Lifestyle and Wellbeing Data" from the Work-Life Balance survey. The survey evaluates how respondents thrive in professional and personal lives along the following dimensions: healthy body, healthy mind, expertise, social connections, and life meaning. This project aims to extract insights that can help optimize employees' work-life balance and increase achievements in professional and personal lives.

Hopefully, this work-life balance and achievement data analysis will help job seekers and employees make some changes in their lives for the better

## Target audience
The target audience is job seekers and employees.

## Dataset
Link for this Kaggle dataset: https://www.kaggle.com/ydalat/lifestyle-and-wellbeing-data
Link for the survey: http://www.authentic-happiness.com/your-life-satisfaction-score

The dataset contains the survey responses from www.Authentic-Happiness.com. Work-Life Balance survey evaluates how we thrive in both our professional and personal lives: healthy body, healthy mind, expertise, social connections, and life meaning. Work-Life Balance Score is based on recent research published in the 360 Living guide. The Work-Life Balance Score is the total of all five categories: a poor score is below 550,  a good score is above 680, and an excellent score is above 700. 

The data set consists of 24 attributes describing how we live our lives, including a calculated field, the Work-Life Balance Score. There are around 15972 rows of data for the period from July 2015 until March 2021.

## Data variables:
- 'FRUITS_VEGGIES': [Between 1 and 5] HOW MANY FRUITS OR VEGETABLES DO YOU EAT EVERYDAY? 
- 'DAILY_STRESS': [Between 1 and 10] HOW MUCH STRESS DO YOU TYPICALLY EXPERIENCE EVERYDAY? 
- 'PLACES_VISITED': [Between 0 and 10] HOW MANY NEW PLACES DO YOU VISIT? Over a period of 12 months.
- 'CORE_CIRCLE': [Between 0 and 10] HOW MANY PEOPLE ARE VERY CLOSE TO YOU? 
- 'SUPPORTING_OTHERS': [Between 0 and 10] HOW MANY PEOPLE DO YOU HELP ACHIEVE A BETTER LIFE? Over a period of 12 months.
- 'SOCIAL_NETWORK': [Between 0 and 10] WITH HOW MANY PEOPLE DO YOU INTERACT WITH DURING A TYPICAL DAY? 
- 'ACHIEVEMENT': [Between 0 and 10] HOW MANY REMARKABLE ACHIEVEMENTS ARE YOU PROUD OF? Over the last 12 months
- 'DONATION': [Between 0 and 5] HOW MANY TIMES DO YOU DONATE YOUR TIME OR MONEY TO GOOD CAUSES? Over a period of 12 months. 
- 'BMI_RANGE': [1 if below 25, else 2] WHAT IS YOUR BODY MASS INDEX (BMI) RANGE? 
- 'TODO_COMPLETED': [Between 1 and 10] HOW WELL DO YOU COMPLETE YOUR WEEKLY TO-DO LISTS? On a scale of 0 = not at all to 10 = very well.
- 'FLOW': [Between 0 and 10] IN A TYPICAL DAY, HOW MANY HOURS DO YOU EXPERIENCE "FLOW"? 
- 'DAILY_STEPS': [Between 0 and 10] HOW MANY STEPS (IN THOUSANDS) DO YOU TYPICALLY WALK EVERYDAY? 
- 'LIVE_VISION': [Between 0 and 10] FOR HOW MANY YEARS AHEAD IS YOUR LIFE VISION VERY CLEAR FOR? 
- 'SLEEP_HOURS': [Between 0 and 10] ABOUT HOW LONG DO YOU TYPICALLY SLEEP? Over the course of a typical working week, including weekend.
- 'LOST_VACATION': [Between 0 and 10] HOW MANY DAYS OF VACATION DO YOU TYPICALLY LOSE EVERY YEAR? Unused vacation days.
- 'DAILY_SHOUTING': [Between 0 and 10] HOW OFTEN DO YOU SHOUT OR SULK AT SOMEBODY? In a typical week. 
- 'SUFFICIENT_INCOME': [1 for insufficient, 2 for sufficient] HOW SUFFICIENT IS YOUR INCOME TO COVER BASIC LIFE EXPENSES? 
- 'PERSONAL_AWARDS': [Between 0 and 10] HOW MANY RECOGNITIONS HAVE YOU RECEIVED IN YOUR LIFE? Over a period of 12 months.
- 'TIME_FOR_PASSION': [Between 0 and 10] HOW MANY HOURS DO YOU SPEND EVERYDAY DOING WHAT YOU ARE PASSIONATE ABOUT? 
- 'WEEKLY_MEDITATION': [Between 0 and 10] IN A TYPICAL WEEK, HOW MANY TIMES DO YOU HAVE THE OPPORTUNITY TO THINK ABOUT YOURSELF? 
- 'AGE’: [1 = 'Less than 20' 2 = '21 to 35' 3 = '36 to 50' 4 = '51 or more’]”,
- ‘GENDER’: [1 = 'Female' 0 = 'Male']

## Resources 
https://www.kaggle.com/ydalat/lifestyle-and-wellbeing-data 
You can download this dataset from Kaggle. Please, see the code below.

import os
for dirname, _, filenames in os.walk('/kaggle/input'):
    for filename in filenames:
        path = os.path.join(dirname, filename)

After downloading the CSV file, I did some preliminary data preparation in Excel, including changing data types for a few variables and lower cases for all column headings.

## Features of interest
- Work-life balance score
- Achievement

## Research questions
- Do the variables in the dataset explain the work-life balance score? 
- Which demographic has the better or worse work-life balance according to this data? 
- Which demographic has the better or worse achievement according to this data? 
- What are the strongest correlations between the various variables? 
- What drives our work-life balance?
- What drives our achievement?
 

## Steps completed
-	Preprocess/ Clean/ Create new variables
-	EDA of work-life balance score and achievement, using Python
-	Visualization of data analysis, using Matplotlib, Seaborn, ggplot 

## Exploratory data analysis
Interesting findings from the dataset:
- 'fruits_veggies' (1-5)  – daily respondents eat 3 fruits or vegetables on average
-  'daily_stress' (1-10)- respondents have level 3 of stress on average daily
- 'places_visited' (0-10) - respondents visit 5 new places on average over a period of 12 months. 22% of respondents travel to at least 10 new places over a period of 12 months
-  'core_circle' (0-10) - on average, respondents have 5 people who very close to them 
-  'supporting_others' (0-10) - respondents support 6 people on average over a period of 12 months
-  'social_network' (0-10) – respondents interact with 6 people every day on average
-  'achievement' (0-10)– respondents proud of 4 achievements per year on average over a period of 12 months
-  'donation' (0-5) – respondents donate their time or money 2 times over a period of 12 months on average 
-  'bmi_range' (1, 2) – 59% of respondents have a healthy weight with bmi range below 25.
-  'todo_completed' (0-10) – respondents complete their weekly to-do list at level 6 on average
-  'flow' (0-10) – 19% of respondents experience only 2 hours of 'flow'. 8% of respondents do not experience 'flow' at all
-  'daily_steps' (0-10) - 17% of respondents typically walk at least 10 thousand steps per day. 8% of respondents walk around one thousand steps per day
-  'live_vision' (0-10) – 16% of respondents have their clear life vision for 5 years ahead, and 16% of respondents have their clear life vision for 0 years
- 'sleep_hours' (0-10) – 70% of respondents sleep 7-10 hours per night. 27% of respondents sleep 5-6 hours per night
-  'lost_vacation' (0-10) – 51% of respondents use all their vacation days. 14% of respondents typically lose 10 days of vacation per year
-  'daily_shouting' (0-10) – 15% of respondents do not shout or sulk at all. 23% of respondents shout or sulk at somebody typically one time per day
-  'sufficient_income' (1, 2) – 73% of respondents have a sufficient income
-  'personal_awards' (0-10) – 24% of respondents obtain at least 10 personal awards over a period of 12 months
-  'time_for_passion' (0-10) – respondents spend 3 hours per day on average doing what they passionate about
-  'weekly_meditation'  (0-10) – 27% of respondents think about themselves at least 10 times in a typical week
-  'work_life_balance_score' (1-3)– Only 0.5% of respondents said they have poor work-life balance. 60% of respondents have a good work-life balance. 39.5% of respondents have an excellent work-life balance

## Do the variables in the dataset explain the work-life balance score? 
The variables in the dataset explain the work-life balance score. From the correlation analysis, we can see that the seven variables have a strong positive correlation with the work-life balance score, eight variables have a moderate positive correlation with the work-life balance, and one variable has a moderate negative correlation. 
"Your Work-Life Balance survey evaluates how we thrive in both your professional and personal lives: it reflects how well you shape your lifestyle, habits, and behaviors to maximize your overall life satisfaction along the following five dimensions:
1. Healthy body, reflecting your fitness and healthy habits;
2. Healthy mind, indicating how well you embrace positive emotions;
3. Expertise, measuring the ability to grow your expertise and achieve something unique;
4. Connection, assessing the strength of your social network and your inclination to discover the world;
5. Evaluate your compassion, generosity, and how much 'you are living the life of your dream.'" (1)
Hopefully, in the future, we will have more available observations and new variables to explore. 

## Which demographic has the better or worse work-life balance according to this data?
- 62% of respondents are women, and 38% are men in our dataset. On average, the work-life balance score between all four age groups and by gender are very similar and varies from 2.3 to 2.5.
- 52% of respondents with sufficient income have a good work-life balance. 48% of respondents with sufficient income have an excellent work-life balance. 1.5% of respondents with insufficient income have a poor work-life balance. 83% of respondents with insufficient income have a good work-life balance. 16% of respondents with insufficient income have an excellent work-life balance.
 
## Which demographic has the better or worse achievement according to this data?
- On average, the achievement between all four age groups and by gender are very similar and varies from 3.8 to 4.4.
- 42% of respondents with insufficient income have 0 achievements in the 12 months. 58% of respondents with sufficient income have 0 achievements in 12 months.
- 18% of respondents who do not have sufficient income have 10 achievements in the period of 12 months. 82% of respondents who have sufficient have 10 achievements in the 12 months.


## What are the strongest correlations between the various variables?
- 'work life balance score' and 'achievement' have the strongest positive correlation of 0.561
- ‘work life balance score’  have a strong positive correlation  above 0.5 with 'supporting_others',  'todo_completed', 'places_visited', 'time_for_passion', 'core_circle', 'personal_awards'.
- ‘work life balance score’ and ‘flow’, 'daily_steps', 'live_vision', 'fruits_veggies', 'sufficient_income', 'weekly_meditation', 'social_network', 'donation' have a moderate positive correlation above 0.4.
- 'time_for_passion' and 'flow' have a moderate positive correlation 0.483
- Daily stress is moderately correlated with daily shouting.
- Lost vacation and gender positively correlated with daily stress.  
- From correlation analysis, we can see that the work-life balance and weekly meditation decrease our daily stress.

## What drives our work-life balance?
- The EDA shows that our work life balance is strongly and positively driven by ‘achievement’ , 'supporting_others' ,'todo_completed' , 'places_visited' , 'time_for_passion' ,  'core_circle' , 'personal_awards' . 
-  ‘work life balance score’ moderate positive depends on ‘flow’, 'daily_steps', 'live_vision', 'fruits_veggies', 'sufficient_income', 'weekly_meditation', 'social_network', 'donation'.
- By supporting others and donating our time and money to others, we improve our work-life balance. 
- Traveling and visiting new places increase the quality of our well-being too. 
- Also, by eating more fruits and veggies, walking more steps, and regularly meditating, we moderately increase our healthy work-life balance. 

## What drives our achievement?
- From this data analysis, we can see that we achieve more when we have a good 'work-life balance. The work-life balance has the strongest correlation with 'achievement.'
- Moderately 'achievement' depends on 'personal awards,' 'time for passion,' and flow.' 
- Also, the more we support others, the more we achieve in our lives.

## Takeaways for job seekers
- The easiest way to improve work-life balance is for job seekers and employees to eat more Fruits and Veggies, Visit new places, even a new coffee shop or hiking trail 5 minutes away, and do more daily steps. Just these habits will make the work-life balance of anyone much better. So, prioritize your health. During the workday, employees should take regular breaks and short walks. It will improve their flow and to-do completion. 
- Meditation can increase healthy work-life balance too. Flow, daily meditation, and sufficient income will decrease daily stress.
-  An excellent work-life balance includes vacation days, time for passions, and hobbies outside of work. Prioritize your quality time to unplug during evenings, weekends, and vacations. It will inspire and recharge you.
- To have high factors to-do completed and life vision, set your professional in personal goals and priorities. Set achievable goals. Know your most productive time of the day and block that time for the most important tasks. It will increase your flow too. 
- Make time for other people, including your loved ones, friends, clients, and colleagues. Data analysis shows us that the more we support others, donate time and money, and have a core circle, the greater our work-life balance. 
- To increase factors "time for passion" and "flow," have or find a job you are passionate about. Employees will be more productive and less stressed.  

## Interesting findings from data:
- 22% of respondents travel to at least 10 new places over 12 months
- 17% of respondents typically walk at least 10 thousand steps per day. 8% of respondents walk around one thousand steps per day
- 16% of respondents have their clear life vision for 5 years ahead, and 16% of respondents have their clear life vision for 0 years
- 70% of respondents sleep 7-10 hours per night. 27% of respondents sleep 5-6 hours per night.
- 51% of respondents use all their vacation days. 14% of respondents typically lose 10 days of vacation per year
- Only 0.5% of respondents said that they have poor work-life balance. 60% of respondents have a good work-life balance. 
- 39.5% of respondents have an excellent work-life balance

## Next steps
- Analyze other work-life balance datasets with other variables, including the level of education, work hours per week, workdays per month, and location of respondents. Combine and compare variables and data analysis results.
- Build a prediction model for a work-life balance score and achievements.
- It might be interesting to build an app that will evaluate a person's work-life balance daily and advise which factors can be improved.
- Ask the HR department to consider the work-life balance score at your company. It can provide additional information for both employers and employees to improve productivity and happiness.

## References:
1. Link for the dataset in Kaggle: https://www.kaggle.com/ydalat/lifestyle-and-wellbeing-data
2. Link for the survey:http://www.authentic-happiness.com/your-life-satisfaction-score
3. https://www.apollotechnical.com/statistics-on-work-life-balance/
4. https://www.businessnewsdaily.com/5244-improve-work-life-balance-today.html
5. https://healthcareers.co/work-life-balance-statistics/
6. https://smartasset.com/data-studies/cities-with-the-best-work-life-balance-2022

