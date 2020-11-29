# Beam programming structure/model

It takes input from different system >> pass it on to beam pipeline it passes through multiple transformation >> finally it produces the outputs.

## Example

From a text file we need to count the attendance of the employee.

### Input file

in CSV format

emp_id, emp_name, dept_no, dept_name, date_present
1234, Abhi, 6, accounts, 01-01-2019

### Steps

We need to count each element, for each employee of accounts department.

1-read the data form the file, and store it in a collection.
2-filter all the employee from collection whose department is accounts and store it in another collection.
3-group-by: based on employee id or name and store it in another collection.
4-sum/count: number of rows for each employee and store it in another collection.
5-output: write it to another file or source.
