# TaCLe
## Experimental data for the TaCLe system and screenshots of the systems

There are three steps to perform learning in tabular data. For a demonstration, have a look at [the gif demonstraiting the process](https://raw.githubusercontent.com/SergeyParamonov/TaCLe/master/screenshots/fruit_demo.gif) (on the fruit.csv) or at the steps separately on the main demo example:

1. Upload the file via web-interface: [image](https://raw.githubusercontent.com/SergeyParamonov/TaCLe/master/screenshots/demo_file.png)

2. Select tables one by one: [selection of one table](https://raw.githubusercontent.com/SergeyParamonov/TaCLe/master/screenshots/demo_selected_first.png), [all tables are selected](https://raw.githubusercontent.com/SergeyParamonov/TaCLe/master/screenshots/demo_selected_all.png)

3. Push *Learn Constraints*: [output](https://raw.githubusercontent.com/SergeyParamonov/TaCLe/master/screenshots/demo_learned.png)

## Examples of learned constraints

The same steps for the different csv file, department.csv, demonstrating the **SUMIF** constraint: [step 1](https://raw.githubusercontent.com/SergeyParamonov/TaCLe/master/screenshots/deparment_1.png), [step 2](https://raw.githubusercontent.com/SergeyParamonov/TaCLe/master/screenshots/deparment_selected_tables.png) and [step 3](https://raw.githubusercontent.com/SergeyParamonov/TaCLe/master/screenshots/deparment_learned.png).

Let us also present some other constraints that can be learned by the system:

* [Fuzzy-lookup](https://raw.githubusercontent.com/SergeyParamonov/TaCLe/master/screenshots/screenshot_fuzzy_lookup_bmi.png) as learned from BMI.csv
* [Rank and series](https://raw.githubusercontent.com/SergeyParamonov/TaCLe/master/screenshots/screenshot_score_series_rank_sum.png) as learned from score.csv
* [Arithmetic expressions](https://raw.githubusercontent.com/SergeyParamonov/TaCLe/master/screenshots/screenshot_belgium_arithmetic_sum.png) as learned from belgium.csv
* [Row and column sums](https://raw.githubusercontent.com/SergeyParamonov/TaCLe/master/screenshots/screenshot_sums_baltimore.png) as learned from baltimore.csv
* [If-aggregates: MINIF, COUNTIF, AVGIF, etc](https://raw.githubusercontent.com/SergeyParamonov/TaCLe/master/screenshots/screenshot_aggregate_if.png) as learned from rides.csv

## Files:  

**links.txt** contains the list of links to the Excel documents collected from the Internet for experiments  

**data.txt** describes the split of documents into three categories (used in the paper in the experimental section)

## Folders: 

**csv** has the original CSV files obtained by converting Excel into CSV (**Removed due to legal reasons of GDPR**) 

**groups** has the description of the groups for the corresponding CSV files in the *csv* folder

**truth** contains the ground truth for the experiments, i.e., the constraints in the Excel documents

## Spreadsheet sources
We collected spreadsheets from three main sources.
* After identifying popular Excel functions, the [MS Office web page](https://support.office.com/en-us/article/Excel-functions-by-category-5F91F4E9-7B42-46D2-9BD1-63F26A86C0EB}) has an overview of popular functions, we searched for online tutorials about these functions and collected them under the category **Tutorials**. A link to each webpage found and used is provided in [links.txt](/links.txt) file.
* We have collected the exercises under the category **Exercises** from the introductory Excel book (MS Excel 2010 by Eddy Van den Broeck and Erik Cuypers) that focused 1) on popular Excel functions and 2) on datatypes supported by our system.
* We have collected under the category **Data** spreadsheets reporting data. More specifically, economic data, crime reporting data and data from runtime experiments. The spreadsheets on economic data and crime reporting are publicly available and originate from the U.S. Bureau of Economic Analysis (BEA), the RWE annual report 2014 and the U.S. FBI Uniform Crime Reporting (UCR) Program.
 

## Constraint distribution across the categories

The technical description of the dataset is summarized in two tables: occurances of constraints in categories and fraction of spreadsheets that has these constraints.

The number of constraint occurances in spreadsheets

| constraint | Data | Tutorials | Exercises | 
| --- | --- | --- | --- |
| average (col) | 0 | 2 | 0 | 
| average (row) | 1 | 0 | 0 | 
| average-if | 0 | 0 | 1 | 
| count (col) | 0 | 1 | 0 | 
| count-if | 0 | 0 | 1 | 
| difference | 1 | 0 | 2 | 
| equal | 0 | 10 | 0 | 
| foreign-product | 0 | 0 | 1 | 
| fuzzy-lookup | 0 | 1 | 2 | 
| lookup | 0 | 0 | 1 | 
| max (col) | 0 | 2 | 0 | 
| max-if | 0 | 0 | 1 | 
| min (col) | 0 | 3 | 0 | 
| min-if | 0 | 0 | 1 | 
| percentual-diff | 1 | 0 | 5 | 
| product | 0 | 3 | 2 | 
| project | 0 | 0 | 1 | 
| rank | 0 | 0 | 1 | 
| series | 1 | 0 | 2 | 
| sum (col) | 0 | 10 | 5 | 
| sum (row) | 2 | 3 | 2 | 
| sum-if | 0 | 9 | 2 | 
| sum-product | 0 | 2 | 0 |


The fraction of spreadsheets containing specified constraints:

| constraint | Data | Tutorials | Exercises |
| --- | --- | --- | --- |
| average (col) | 0.00 | 0.10 | 0.00 | 
| average (row) | 0.25 | 0.00 | 0.00 | 
| average-if | 0.00 | 0.00 | 0.11 | 
| count (col) | 0.00 | 0.05 | 0.00 | 
| count-if | 0.00 | 0.00 | 0.11 | 
| difference | 0.25 | 0.00 | 0.22 | 
| equal | 0.00 | 0.24 | 0.00 | 
| foreign-product | 0.00 | 0.00 | 0.11 | 
| fuzzy-lookup | 0.00 | 0.05 | 0.22 | 
| lookup | 0.00 | 0.00 | 0.11 | 
| max (col) | 0.00 | 0.10 | 0.00 | 
| max-if | 0.00 | 0.00 | 0.11 | 
| min (col) | 0.00 | 0.14 | 0.00 | 
| min-if | 0.00 | 0.00 | 0.11 | 
| percentual-diff | 0.25 | 0.00 | 0.11 | 
| product | 0.00 | 0.14 | 0.11 | 
| project | 0.00 | 0.00 | 0.11 | 
| rank | 0.00 | 0.00 | 0.11 | 
| series | 0.25 | 0.00 | 0.22 | 
| sum (col) | 0.00 | 0.33 | 0.56 | 
| sum (row) | 0.25 | 0.14 | 0.22 | 
| sum-if | 0.00 | 0.38 | 0.22 | 
| sum-product | 0.00 | 0.10 | 0.00 |
