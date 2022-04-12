# Capstone-Research-Paper-2021
Using information dowloaded from the American Community Survey, Federal Reserve Economic Data, and Official NYC zcta and zip datasets.

# ETL dataset manipulation in R
In this file I have dowloaded all workbooks and manipulated the files in the following way to create an official dataset for analysis:
  1. Formatting Aldi workbooks for merger 
    a. Aldi locations workbook import   
    b. 'zip' to numeric 
    c. 'zip' to 'zcta' conversion
  2. Download from 2011 workbook and 2012-2019 workbooks
    a. File imports 2011 - 2019 
    b. Get all desired variables from 2011-2019 workbooks
  3. 2011 - 2019 Panel Compilation and Cleanup
    a. Create one df
    a. Removing all non New York State Locations
    b. Converting all columns numeric except 'county' and 'stab'
    c. Delete zctas with missing information
    d. Set 'id' as primary key
    e. Set 'aldi' as indicator var
    f. Format County values to not contain 'NY', and hyphenate between words
    g. Add NY regions, and formulate numeric codes for counties and regions
    k. Adjust housing values and incomes for inflation
  4. Reorder columns
  5. Export to Excel File
