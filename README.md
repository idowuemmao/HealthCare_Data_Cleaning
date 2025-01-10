# HealthCare_Data_Cleaning
A dive into data cleaning with power query and excel.

NOTE: Before commencing with the data cleaning in Date of Admission column I manually replaced the date in word format to the actual date, while the date in number format I highlighted and change type to short date in excel, I also changed the data type of salary to general to change negative values from (100) to -100 before beginning the cleaning in Power Query.
I did this because the number of dates to change wasn’t much, if it was more than expected I would have taken a different approach with formulas.
1.	ID: I did no correction for the ID column, but I noticed some duplicates in the ID
2.	Name: Using the transform tab I 
- Capitalized each word using – Transform > Format > Capitalize Each Word
- Trim text in column to remove white space.
3.	Age: Using the transform tab I 
- Replace value Unknown with 0
4.	Gender
- Replace value M with Male, and selected Match entire cell contents in the Advanced options.
- Replace value F with Female, and selected Match entire cell contents in the Advanced options.
- Replace blanks with Others
5.	City: Using the transform tab I 
- Replace “Albuque” with “Albuquerque”, and selected Match entire cell contents in the Advanced options.
- Replace “Atl” with “Atlanta”, and selected Match entire cell contents in the Advanced options.
- Replace “Balti” with “Baltimore”, and selected Match entire cell contents in the Advanced options.
- Capitalize each word
6.	Blood Type: Using the transform tab I 
- Replace blanks with None
7.	Education: Using the transform tab, I 
- Replace blanks with None
- Replace ‘s with blank
8.	Employment Status:
- Using Add column I extracted text between delimiter ( and ) to extract the text between them
- I renamed the column to Employment Type
- I reordered the column to be beside each other
- Extracted text before delimiter “(“ in Employment Status to remove the text in the bracket 
- I trimmed text in Employment status column to remove whitespace
- In Employment type column replace blank with None
9.	Salary
- Replace $ with blank to remove it
- Using Add column I extracted text before delimiter ( and ) to extract the text between them.
- Renamed the column as Salary Structure
- Reorder the column to be close to each other.
- Extract text before delimiter ( to remove unnecessary text in salary column
- Replace “Missing” with 0 
- Replace blank with 0
- Replace blanks in salary structure with None
10.	Health Condition:
- Extracted Text Before Delimiter (
- Trimmed Text in Health Condition
- Replaced blank with None
11.	Health Condition
12.	Credit Score
- Extracted Text Before Delimiter ‘(‘ to remove the (typo)
- Trimmed text
- Replace N/A with 0
- Replace none with 0
- I highlighted the whole column and Detect Data Type in Transform tab

Further Steps taken in Excel highlighting 
- Highlighted the entire table and remove duplicates from the Data tab, highlight all columns and click Ok. 3 duplicate values found and removed; 1656 unique values remain
- I Highlighted the Age below 18 to confirm the authenticity of the data.
