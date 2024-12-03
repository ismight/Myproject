## CAPSTONE PROJECT
### Project Overview
 - This Project is a capstone Project that intents to give in depth analysis on `healthconnect` a company
providing innovative healthcare solutions. The project is designed to analyze patient data,
discover trends, and build insightful dashboards to aid management in decision-making.
#### Project Objectives
- To Analyze the organization’s patient database to discover trends and
insights. 
- The company is interested in identifying common health issues,
treatment outcomes, and geographical distribution of diseases to better tailor its
services.
#### Project Dataset Gathering $
- The company dataset was provided and was dowloaded from kaggle with medical cost dataset was as well downloaded as required. The dataset include anonymized patient data,
including variables such as `age`, `gender`, `region`, `symptoms`, `diagnosis`, `treatment
plan`, and `outcomes`.
#### DATA EXPLORATION AND CLEANING:
- After the datasets was downloaded, they were loaded in [Microsoft excel](www.microsoft.com/excel) , where;
- I. Duplicates was first removed using the `Name column` in the Healthcare dataset, this allow the 
duplicate values to be removed in other column of the same table.
- II. The `name column` was changed from improper text to a proper text format, using a proper 
function (i.e, =proper(text)) which change the name column details into proper text.
- III. The billing amount was formatted as currency as well as the admission and discharge date
- IV. The data was therefore, saved.
- V. In the SQL,
- VI. After the two data was imported in the ‘capstone database’, 
- VII. `Select * from healthcare` was executed so as to verify the datasets.
- VIII. However, `select top 1000 from name,age, gender,blood type` etc from the healthcare datsets 
was identified while only the region was selected from the medical_cost table
- IX. Then a `left join healthcare table on medical_cost.age = healthcare.age` was executed. This 
query help to bring the top 1000 row of the healthcare table which was left join with the 
medical cost region so as to retrieve the 2 table as one table thereafter.
- X. Therefore, the dataset table result was saved as csv for the power bi visualization.
#### DATA ANALYSIS:
The descriptive analysis; 
- I. The most common diagnosis by region is `asthma`, this was achieved by using a quick measure, 
where medical condition was used and categorized with count of medical condition by region
- II. Success rates by diagnosis was achieved by determine the duration of stay, this is achieved by 
Datedif function on (day of admission and discharge date) to each date. However, with the 
count function on Medication, Aspirin happened to be the best medication with average of 132 
days to treat any medical conditions. Follow by ibubrofen (138), paracetamol (206), lipitor(212) 
and pencillin (312).
- III. Demographic of patients with specific health condition is achievable by grouping the age into 
group as (0-20), (21-40) and (60 and above). However, age 21-40 appear to have all the medical 
conditions, 41-60 have just five medical condition with no arthritis while age 60 and above have 
only just 2 medical condition which are asthma and cancer.
#### DATA VIZUALIZATION
- 1) A Bar chart was used to visualized this, the legend are 
I. Light blue for age 21-40 which happened to be the highest age with much of medical 
condition 
II. Navy blue is 41-60
III. Yellow rep 60 and above which rep the least of the medical condition of patient
Therefore age demographic was used with the medical condition of the patient as the basis for this 
visualization
- 2) A pie chart was used to know visualized the rate by days of each medication to treat any medical 
conditions. 23.64% represent aspirin, 21.24% represent ibuprofen, 20.52% Lipitor, 102.61%
represent paracetamol while 14.98% represent penicillin.
- 3) A map was used to represent geographical distribution of health condition in each region. 
Medical conditions were used as the legend to show the area at which each condition is located.
- 4) Scatter chart was used for the regression analysis and it shows the medication have more 
positive effect on male.
![visualised image](<img width="512" alt="Screenshot 2024-11-26 092205" src="https://github.com/user-attachments/assets/d1667d7f-8d43-4668-ae75-8ae1f875b85f">)
#### Reeconmmendation
- From the analysis, it can be deduced that, any age that falls within 21-40 have been diagnosed more with all the medical conditions. Therefore, the teenagers needs to be oriented and re-oriented on the importance of health conditions which they need to be attentive to their medical conditions.
- Also, Aspirin needs to be produced more and give more attention as the major traetment that help to solve most of the medical conditions.
- Lastly, There is need for the efficiency of international organisation, forexample, UNESCO, WHO and more regeional health organisation on restrategies which can help to eradicate or reduce the imposition of variiety of all the diagnosis in different countries base on the diagnosis domination.
#### References
[kaggle](www.kaggle.com/dataset)

