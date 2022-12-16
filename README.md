# Survival-Analysis

 Three data-sets have been considered for this task:
 MSK
 GENIE
 TCGA
 
# MSK-IMPACT DATA-SET
Data- sets: 
1.  Data Clinical patient : Give descriptions of all columns
2.  Data Clinical Sample
3.  Data mutation
4.  Output_9606.protein.links

# Procedure
Step 1: Merging above datasets

Step 2: Boostrap dataset into train and test split

Step 3: Selecting one of the cancer type =”Breast”

Step 4: Duplicate records for patient ids are dropped.

Step 5 : Grouping all the genes that are mutated corresponding to unique patient ids. :: biological significance?? 

Step5: Created Protein-Gene mapping Output file from Python code (Another Python notebook) :
biological significance: We have superset of protein-protein network but we have gene level inforamtion for patient. Hence, to map this gene information to protein super-set network we did this mapping using code. File was pre-processed to handle messy data before running the code.

Step6: Pre-processed above file obtained
This was done to ensure that all those proteins that are mapped to genes above should only be considered as standard, anything else included in list of mutated genes of patients should be dropped off.

Step8: Calculate Sg values for both train and test
(what is sg value and what is it significance??)



Step9: Switching To R Code-RWR
•	I/P- Sg values of train data
•	Seed of test data: Gene list of patients of test data
•	With the help of code variable length seed was handled
•	Dataframe was being created to store Rwr Score, Node Name in ascending for Top k genes for train data. 
•	Then, check if  test data genes that are present as seed to RWR in merged data and calculate average of it. 
Biological Significance:This will give us a hint that if a gene is mutated then based on this action, other genes that will also be mutated.

Step10: Output obtained from RWR code that has records as same as that of the number of records in the seed of RWR.

Step11: Calculate median value and put for threshold.

Step12: Survival Analysis code
I/P- Threshold value from Python code
Kapler meyrs plots


