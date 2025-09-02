## Formated Headings
1. Fonts: Segoe Semibold UI
2. Font Type: Bold
3. Font Color: White
4. Fill Color: Green

## Removing Null Values (Blank Rows/Cells)
1. Dataset Shape: *6704 × 6*

2. Identified blank rows using
<p align="center">
    <em>(Ctrl + G) → (Special) → (Blanks)</em> 
</p>

3. Then deleted blank rows using
<p align="center">
    <em>(Ctrl + -) → (Entire Row)</em>
</p>

4. Dataset Shape After Removing Blank Rows: *6698 × 6*

## Removing Duplicates
1. The dataset contains 4911 duplicates. Duplicates are identified from the 
<p align="center">
    <em>(Data Tab) → (Remove Duplicates) → (Select All Columns)</em>
</p>

2. Dataset Shape After Removing Duplicates: *(1787 × 6)*

## Renaming Redundant Entries
1. Dataset Headings: *Age*, *Gender*, *Education Level*, *Job Title*, *Years of Experience*, and *Salary*
2. *Education Level* column contained redundant entries such as *Bachelor's Degree*, *Bachelor's*, *Master's Degree*, *Master's*, etc. Renamed *Bachelor's Degree* → *Bachelor's* and *Master's Degree* → *Master's* by 
<p align="center">
    <em>Editing → Find & Select → Replace from Home Tab</em>
</p>
    
3. Created a table named <em>Cleaned_Data</em> after data cleaning and saved a pdf version of the table on *./Reports/Pre_Processing_Report/Cleaned_Dataset.pdf*