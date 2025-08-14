## Formated Headings
1. **Fonts**: Segoe Semibold UI
2. Font Type: Bold, Font Color: White, Fill Color: Green

## Finding 1
1. Dataset Shape: 6704 rows (Excluding Headings) and 6 columns
2. Identified blank rows using *(Ctrl + G)* → *(Special)* → *(Blanks)*. Then deleted blank rows using *(Ctrl + -)* → *(Entire Row)*
3. Dataset Shape After Removing Blank Rows: *(6698 × 6)*

## Finding 2
1. The dataset contains 4911 duplicates. Duplicates are identified from the *(Data Tab)* → *(Remove Duplicates)* → *(Select All Columns)*
2. Dataset Shape After Removing Duplicates: *(1787 × 6)*

# Finding 3
1. Dataset Headings: *Age*, *Gender*, *Education Level*, *Job Title*, *Years of Experience*, and *Salary*
2. *Education Level* column contained redundant entries such as *Bachelor's Degree*, *Bachelor's*, *Master's Degree*, *Master's*, etc. Renamed *Bachelor's Degree* → *Bachelor's* and *Master's Degree* → *Master's* by *Editing* → *Find & Select* → *Replace* from *Home Tab*
3. Saved the cleaned dataset in pdf format on *./Reports/Dataset/Cleaned_Dataset.pdf*