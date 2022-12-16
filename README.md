# Survival-Analysis

 Three data-sets have been considered for this task:
 
 
MSK-IMPACT DATA-SETS
Data- sets: 
1.  Data Clinical patient : Give descriptions of all columns
2.  Data Clinical Sample
3.  Data mutation
4.  Output_9606.protein.links

## Procedure
Step 1: Merging above datasets
Step2: Boostrap dataset into train and test split
Step 2: Selecting one of the cancer type =”Breast”
Step3: Duplicate records for patient ids are dropped
Step4 : Grouping all the genes that are mutated corresponding to unique patient ids. :: biological significance?? 
Step5: Created Protein-Gene mapping Output file from Python code (Another Python notebook) :
biological significance: recheck this
Step6: Pre-processed above file obtained. 
Why???messy data
Step7: Deleting genes from patient id that are not in Output 9606 files.
Step8: Calculate Sg values for both train and test
(what is sg value and what is it significance??)
Step9: Switching To R Code-RWR
Apart from RWR what else can be applied and how??
•	I/P- Sg values of train data
•	Seed of test data: Gene list of patients of test data
•	With the help of code variable length seed was handled
•	Dataframe was being created to store Rwr Score, Node Name in ascending for Top k genes for train data. ( why top k??)
•	Then, check if  test data genes that are present as seed to RWR in merged data and calculate average of it. (why??)
Step10: Output obtained from RWR code that has records as same as that of the number of records in the seed of RWR.
Step11: Calculate median value and put for threshold. (Quartiles/Quantiles):::::::research paper 
Step12: Survival Analysis code
I/P- Threshold value from Python code
Kapler meyrs plots


