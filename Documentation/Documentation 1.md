## Formated Headings
1. **Fonts**: Segoe Semibold UI
2. Font Type: Bold, Font Color: White, Fill Color: Green

## Finding 1
1. Dataset Shape: 6704 rows (Excluding Headings) and 6 columns
2. Identified blank rows using
<p align="center">
    <em>(Ctrl + G) → (Special) → (Blanks)</em>
</p> 
Then deleted blank rows using 
<p align="center">
    <em>(Ctrl + -) → (Entire Row)</em>
</p>

3. Dataset Shape After Removing Blank Rows: *(6698 × 6)*

## Finding 2
1. The dataset contains 4911 duplicates. Duplicates are identified from the *(Data Tab)* → *(Remove Duplicates)* → *(Select All Columns)*
2. Dataset Shape After Removing Duplicates: *(1787 × 6)*

## Finding 3
1. Dataset Headings: *Age*, *Gender*, *Education Level*, *Job Title*, *Years of Experience*, and *Salary*
2. *Education Level* column contained redundant entries such as *Bachelor's Degree*, *Bachelor's*, *Master's Degree*, *Master's*, etc. Renamed *Bachelor's Degree* → *Bachelor's* and *Master's Degree* → *Master's* by *Editing* → *Find & Select* → *Replace* from *Home Tab*
3. Saved the cleaned dataset in pdf format on *./Reports/Dataset/Cleaned_Dataset.pdf*

## Finding 4
1. Identified data types of each column using a nested formula. For identifying text, *=ISTEXT()* formula is used. Similarly for number, *=ISNUMBER()* is used. The range (A2:A1788 for Age and so on) was given inside the formulas. These formulas were used inside the *=IF()* formula to check if it is a number or a text. Example formula is:
<p align="center">
  <em>=IF (ISNUMBER (A2:A1788), "Number", "NaN")</em>
</p>

2. Complete report of the data types is saved on *./Reports/Data_Types.pdf*
