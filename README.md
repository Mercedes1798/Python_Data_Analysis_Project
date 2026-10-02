# Python for Data Analysis - Course Project
This is the project at the end of the Python for Data Analysis course from Luke Barousse - the course of which I uploaded notes for earlier. The project is based on answering 3 key questions using the skills learned throughout the course.

1. What are the most in-demand skills for the top 3 most popular data roles?
2. How do skills, including the most popular skills, relate to job pay?
3. For Data Analysts in Germany, what are the skills that are both high-demand AND high-pay?

The course project presented here is not exactly the same as the one presented in the YouTube tutorial. I, for instance, decided to exclude one of the key questions because the answer didn't seem particularly insightful, and I the analysis is grounded on data based on job postings in Germany (as opposed to the USA).
I've collected below what I believe to be the most important/insightful graphs and code snippets, along with my own interpretations of the data. 

## I. Most In-Demand Skills
<img width="623" height="472" alt="Hbar 1" src="https://github.com/user-attachments/assets/13e1ae51-bbee-4ac6-bfd3-88dc77ba8d70" />

Above we have the 3 most popular data job titles in DE along with their most sought-after skills presented as a percentage of skill demand over total job postings of the same title. E.g. for data scientist positions, Python is mentioned in the job listing 62% of the time. 

### Quick Insights
- SQL and Python are relevant for all 3 titles; they are the most sought-after skills across the board. Learning these skills is *still* worth your time and effort even as AI takes over the world.
- Since this was a Python for data analysis course: Python comes up in every one in three job openings for data analysts. The only skill more "valued" than Python is SQL, which itself has a very similar syntax to Python's. If you can write code in Python, you can easily leaern to write code in SQL.
- Microsoft applications are still relevant to data analysts; Excel and PowerBI appear in approx. every one in five job listings. 
- Data Engineer and Scientist positions require more cloud skills; Analyst requires more analytical and visualization tools.

## II. Skills and their Pay
<img width="622" height="463" alt="image" src="https://github.com/user-attachments/assets/ca9985ee-051c-40ec-80a5-59622c89fd2a" />

The graph above narrows down data jobs to data analyst jobs in DE only. We're looking at sought-after skills for these positions, but this time with the additional filtering criterion of salary. The upper bar chart presents the skills with the absolute highest associated median salary; the lower bar chart presents the highest-paid but also most frequently appearing (i.e. sought-after) skills.

### Quick Insights
- Besides from GitHub, the absolute highest-paid skills are rather niche. And looking closer at the data, these are skills with a very low frequency i.e. they appear in very few job postings.
- The skills that are both in-demand and have the highest associated median pay are almost the same as the ones we saw in the previous graph on absolute high-demand; instead of PowerBI we have R.
  - Even though SQL came up more often than Python in total data analyst listings, Python has a higher associated median pay.
- Even though Excel is sometimes considered outdated, the data tells us it is not only still required for data analyst jobs, it also still pays to learn it.

## III. Optimal Skills
Now that we've seen what skills are asked for the most along with their associated salary, it begs the question: what are the absolute best skills to learn for a(n) (aspiring) data analyst in DE? We already have the data for this question; it's a matter of how we arrange it for visualization that will help us get a clear answer. 

<img width="624" height="464" alt="image" src="https://github.com/user-attachments/assets/c1adba61-fd24-4a4b-b226-3b6493254a6e" />

The scatter plot above presents us skills that come up in at least 5% of data analyst positions in DE (a total of 15). The frequency of appearance is plotted against associated median salary. Moreover, the skills have been color coded according to skill type/category. 

### Quick Insights
- Most of the skills are grouped in the lower left quadrant meaning lower pay and lower frequency. However, if we regard GitHub as an outlier and adjust the graph quadrants accordingly, many of them are grouped in the upper left quadrant i.e. lower frequency but higher pay.
  - I suggest to disregard GitHub because its associated pay is almost $40K above the next highest-paid skill (gcp) and as I mentioned earlier, it doesn't come up that often anyway; it's skewing our plot.
  - GCP pays but it's not a highly demanded skill.
  - The skills on the upper right quadrant are tableau, python, and sql, meaning they are the skills that are simultaneously sought-after and well-paid i.e. the optimal skills.
  - According to this plot, SQL is the absolute best skill to learn, followed by Python. *The degree of mastery of the skill is not known, however.

## Room for Improvements/Outlook
As I worked my way through this project, I noticed that there were some things that could be improved, namely:

- Convert the salary currency to euros.
- There were a total of 7131 data analyst job listings in DE in the original data set, yet only a meager 48 of them had salary information. There's not much to do about the scarce availability of salary information, it's probably a cultural thing. However, 48 is very small sample size. I would be interesting to conduct a similar analysis to the one presented in the course and final project with a data set that somehow fills in the missing salary data or simply seeks insight not related to salary. 
