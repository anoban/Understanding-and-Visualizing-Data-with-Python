# ___Data Management & Manipulation___
----------------------

## ___Data Management___
----------------

- Data management refers to all apsects of data processing that takes place once all the data have been collecetd but beofre the actual analysis step.

- Most statistical software operates on tabular data, where variables are in columns and observations (records) are in rows.

- A typical rectangular (tabular) data:


| ID      | Age       | State     |
| :---    |    :----: |   ---: |
| 1234D   | 89        | OK   |
| 6647D   | 18        | NY      |
| 6547D   | 36        | LA      |
| 3447D   | 25        | CA      |
| 6601D   | 19        | CO      |
| 6747D   | 24        | MI      |

## ___Best Practices for Data Management___
--------------------

- Never modify the original data files.
- Write a script / programme that analyses the data, without making any in-place modifications.

### ___Advantages___

- New data of similar / identical structure can be analyzed using existing scripts.
- Complex data management can be easily replicated through the documented code.

### ___Best Practices___

- Name variables with interpretable names.
- Short variable names are less informative, long variables names make for less readable code, particularly in complex programmes.
- White spaces are not allowed in variable names in any descent programming language.
- We have the freedom to specify how to treat missing values.

### ___Spreadsheet softwares___

 - Useful for quick anlyses and manual data entry.
 - Limited capabilities in dealing with advanced wrangling & analytics.
 - Encoding information in colours / fonts / other types of formatting will be lost when loaded by data wrangling libraries.
 - Graphs & charts are typically ignored by data wrangling libraries.
 - Each worksheet in a workbook is loaded as separate sheet.
 - Python can read most spreadsheet files, leveraging 3rd party libraries.
 - However, using pure textual/binary data like .csv / .dat / .tsv / .txt is a much safer bet.
 
 ### __Repeating records___
 
 - Wide format data - one row per subject (caregory)
 - Long format - one row per measurement (observation)

___Table below shows the average BMI's of people in specified age intervals___

| Name | Birth State | BMI 0-25 | BMI 25 - 35 | BMI 35 - 45 | BMI 45 - 55 |       
| :---    |    :----: |   ---:  |        ---: |        ---: |        ---: |
| John | OK          |  27.76   | 18.7676     | 23.06       | 19.867      |         
| Kate | MI          |  23.71   | 17.5246     | 12.126      | 26.867      |
| Natalie | CA          |  23.71   | 17.5246     | 12.126      | 26.867      |

- Note that, the there are many Johns from OK as well as CA.
- Average BMIs of John s in the age group 0 - 25 is given in the third column.
- Average BMIs of John s in the age group 25 - 35 is given in the fourth column.

___The corresponding long format of this data will be___

| Name | Birth State | BMI | Age |
| :--- | :---------- | :-: | :-- |
| John | OK          | 18.90 | 40 |
| John | OK          | 12.90 | 29 |
| John | MI          | 23.90 | 17|
| John | CA          | 15.90 | 22 |

- In long format every observation is given a separate row.

## ___Wide format is more covenient for data entry___
## ___Long format more naturally fits many forms of statistical analyses, such as regression analyses.___