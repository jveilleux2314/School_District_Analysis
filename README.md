# School_District_Analysis
# Purpose
I was given the task of analyzing multiple schools in a district to help the school determine passing rates between reading and math, and also determine funding based off those scores. We ran into a dilema after the initial analysis because the 9th grade class of Thomas High School was input incorrectly so I had to exclude that data and re-run so that we had accurate information to base our funding off of. 
# Process
### Changes to _Thomas High school_ since the grades for the 9th grade were inputted incorrectly:

- [x] Locate Thomas High School, 9th Grade - Reading and Math Scores:
- [x] Reading: student_data_df.loc[(student_data_df["school_name"] == **"Thomas High School"**) & (student_data_df **["grade"]== "9th"**), **["reading_score"]]=np.nan**
- [x] Math: student_data_df.loc[(student_data_df["school_name"] == **"Thomas High School"**) & (student_data_df **["grade"]== "9th"**), **["math_score"]]=np.nan** 


### The _tail_ of this data shows the 9th grade reading and math scores to be replaced with NaN:  

<img width="1128" alt="Screen Shot 2021-04-03 at 10 08 04 AM" src="https://user-images.githubusercontent.com/78769464/113483785-d5d6cb00-946a-11eb-979d-9dcbc5a7db63.png">

### From here:
- [x] Created new school data to show the totals & percentages with Thomas High School, 9th grade excluded.
- [x] Compare the top 5 schools to the bottom 5 schools.
- [x] Broke down all of that by school name and started working on spending budgets 

<img width="1140" alt="Screen Shot 2021-04-03 at 1 28 15 PM" src="https://user-images.githubusercontent.com/78769464/113487992-e2661e00-9480-11eb-920e-6e5d88ec8dae.png">


### Here are the top and bottom five schools after factoring out the 9th grade scores of Thomas High School:

<img width="1123" alt="Screen Shot 2021-04-03 at 12 46 26 PM" src="https://user-images.githubusercontent.com/78769464/113486915-ae87fa00-947a-11eb-99fe-ad14efd7d855.png">

### I further analyzed it by school size and school type:
<img width="780" alt="Screen Shot 2021-04-03 at 1 34 19 PM" src="https://user-images.githubusercontent.com/78769464/113488091-8bad1400-9481-11eb-8bc1-b43f69a8d635.png">

<img width="727" alt="Screen Shot 2021-04-03 at 1 36 16 PM" src="https://user-images.githubusercontent.com/78769464/113488111-a2ec0180-9481-11eb-9798-e59de8f2dde1.png">


### School District Summary with new variables:

<img width="1007" alt="Screen Shot 2021-04-03 at 1 00 43 PM" src="https://user-images.githubusercontent.com/78769464/113487844-0412d580-9480-11eb-911f-e49303990bea.png">


Before THS change | After THS Change
------------ | -------------
<img width="994" alt="Before THS Change" src="https://user-images.githubusercontent.com/78769464/113488655-0a578080-9485-11eb-838f-6fedd1b3bf80.png">
<img width="996" alt="After THS change" src="https://user-images.githubusercontent.com/78769464/113488882-771f4a80-9486-11eb-9cb2-b82f06e76a75.png">

# Results 
+ The averages and overall percentage values of Thomas High School changed minimally
+ The budgeting at Thomas High School did not change
+ The other schools did not change either

# Summary

The major changes to the data include : Average math and reading scores, percentage passing of math and reading and overall percent passing at Thomas High School. The overall budgetting was not affected because we did not decrease the amount of students at Thomas High School, we only excluded their scores from Thomas High school's overall results. Although the numerical value of change was minimal- this change allows us to have accurate data and prevents furture errors if re-analyzed later. The passing analysis allows us to see which schools need more funding to allow for more materials to acheive a higher success rate. 




