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
    
3. Created a table named <em>Cleaned_Data</em> after data cleaning and saved a pdf version of the table on *./Reports/Dataset/Cleaned_Dataset.pdf*

## Checking Outliers on Numerical Columns
1. Numerical columns in the cleaned dataset are: *Age*, *Years of Experience*, and *Salary*. Created a table named *Outlier* using these columns. To determine the outliers, the following metrics are required:
<ul>
    <li>*Q1 (First quartile of the individual columns) = {=QUARTILE.INC(Table_Name[Column_Name], 1)}*</li>
    <li>*Q3 (Third quartile of the individual columns) = {=QUARTILE.INC(Table_Name[Column_Name], 3)}*</li>
    <li>*IQR (Inter Quartile Range) = {=Q3 - Q1}*</li>
    <li>*Lower Limit = {=Q1 - 1.5 × IQR}*</li>
    <li>*Upper Limit = {=Q3 + 1.5 × IQR}*</li>
</ul>
