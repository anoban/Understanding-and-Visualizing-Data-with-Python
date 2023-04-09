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