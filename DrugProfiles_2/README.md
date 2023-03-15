Minjun 3rd Year project

Using the jupyter-notebook implimented from https://github.com/MarinaKrivova/DrugProfiles_2
Finding improvement and applying the deep-profiling method
---------------------
analysing given data

-Cosmis ID:
specific genomic location

:: identification of cancer cells
:: each cancer cell has different cosmic id

-Drug ID:
:: identification of drug
:: for some reasons, some drugs have more than one ids
Although this will not be a problem in drug response because on the cell_line data, they use the name of the drug, and to distinguish a drug, PubChem is the most effective way.

-Puchem (id)
:: a special code for a drug
:: there is a python library which has the largest collection of chemical data.
:: there are almost all of the PubChem id for the drugs that are being used in this project
+ There are about 15 drugs that are not found while running the code. So to improve the prediction, it would be better to include these data. I may add the PubChem id for these drugs manually

-Sanger Model

::I have not quite understood it properly, but it seems like a code for a machine-learning model for this project
:: Maybe this could be a standard for comparing the prediction model with my DeepProfiling model

-------------------
Before merging the data
- 



---------------
Marina's goal
1. find out pubchem id for the drugs used in drug profiling
2. remove records with drugs that do not have a reported pubchem id
3. perform filtering of the rest data to leave only valid sigmoid drug response curves
4. divide the rest filtered data into train, validation and test splits according to the number of drug profiles for a certain drug
