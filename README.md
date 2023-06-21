# LinkedIn Data Analyst Jobs

## Description
As the world of data analytics constantly evolves, so do the required skills and knowledge of data analysts. It can be hard to stay up to date on what companies need from their analysts with so many skills and tools to choose from.

I wanted to know what skills companies in my area wanted from their analysts, so I could further guide my own learning and projects and become a stronger candidate when applying.

## Project Info
This project searches public job data from LinkedIn using the following parameters:
-Keyword: Data Analyst 
-Location: Chicago, IL 
-Date Posted: Posted in past 24 hours 
-Area: Within 25 miles 
-Experience Level: Entry level

Once a day, data from the results are scraped using selenium, and formated into a pandas dataframe. This dataframe is exported as a csv and saved. (See ETL.ipynb)

The resulting csvs are loaded into a single dataset, where I use pandas, matplotlib, and other packages to analyze the results. I look at the amount of new jobs per week, common job titles, common skills listed in the job descriptions, and plot the location of the jobs on a map. (See Analysis.ipynb)

## Challenges
An issue I ran into with the data extraction is that LinkedIn will eventually want you to sign in to continue viewing job postings. This happens while looping through each job link and extracting additional info. That is why rows towards the bottom of each days export may lack additional data. As of this latest update, this affects around 14% of the job links in the data.

## Potential Improvements
Eventually, I'd like to move this data to a data warehouse instead of storing on my local machine with csvs. This way the data can be queried with SQL and visualized with a BI tool. 

Also, I'd like to analyze word pairs in the job descriptions, instead of single words. This way terms like "power bi" will show up as one term instead of two.

## Credits
I'd like to credit the following creators whose content assisted with this project.
Luke Barousse - https://www.youtube.com/@LukeBarousse
John Watson Rooney - https://www.youtube.com/@JohnWatsonRooney
Absent Data - https://www.youtube.com/@absentdata