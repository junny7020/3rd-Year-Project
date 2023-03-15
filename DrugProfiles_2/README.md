Minjun 3rd Year project

Using the jupyter-notebook implemented from https://github.com/MarinaKrivova/DrugProfiles_2
Finding improvement and applying the deep-profiling method

-------------------------------
Improvement that has been made <br>
 used gdsc2 for the data as well<br>
 modeled the deep profiling<br>
 
 -------------------------
The next thing to do <br>
fix the code in deep profiling
- error on running on colab

update the versions on colab
- download the files and update the progress


------------------------
+Use of the given data (Ones that were hard to understand)

Cell_Line_Features_PANCAN_simple_MOBEM.tsv:<br>

On the first column-> part of the DNA that has been mutated<br>
On the first row-> there is a list of long digits of numbers (Cosmic ID)<br>
Meaning this is a table of cancer cells(Cosmic ID) indicating which part of their DNA has been mutated.<br>
This will be used for the feature of cancer_cells<br>


---------------------
+Features of data



-Cosmis ID:<br>
Specific genomic location<br>
identification of cancer cells<br>
each cancer cell has a different cosmic id<br>



-Drug ID:<br>
identification of drug<br>
for some reason, some drugs have more than one ids<br>
Although this will not be a problem in drug response because on the cell_line data, they use the name of the drug, and to distinguish a drug, PubChem is the most effective way.<br>



-Puchem (id)<br>
a special code for a drug<br>
there is a python library which has the largest collection of chemical data.<br>
there are almost all of the PubChem id for the drugs that are being used in this project<br>

+ There are about 15 drugs that are not found while running the code. So to improve the prediction, it would be better to include these data. I may add the PubChem id for these drugs manually.<br>



-Sanger Model<br>
I have not quite understood it properly, but it seems like a code for a machine-learning model for this project<br>
Maybe this could be a standard for comparing the prediction model with my DeepProfiling model<br>

-------------------
Before merging the data<br>
- 


--------------------
-


---------------
Marina's goal
1. find out the PubChem id for the drugs used in drug profiling
2. remove records with drugs that do not have a reported PubChem id
3. perform filtering of the rest data to leave only valid sigmoid drug response curves
4. divide the rest filtered data into train, validation, and test splits according to the number of drug profiles for a specific drug
