# Python-for-monthly-recap-from-XLSX-case-1-
Monthly XLSX recap from unstructured Folder directory with Python 

## Description
This simple program is use to help recapitulation process for some value that was input from many corporate office branch/area.
Existing process was do manually copy from XLSX (branch) to master report XLSX, this program is cut that process.
Because of directory unconsistency structure, this program use 'os.walk' to reach the files. 

Program Flow 
1. Input : Report Period
2. Import Files : all XLSX Branch Report data in period 
3. Method:
    a. Read set of cell values from current branch, loop for next branch
    b. Append proccess (3.a.) to dataframe
    c. Drop duplicates, based on latest modified
    d. Export to XLSX
