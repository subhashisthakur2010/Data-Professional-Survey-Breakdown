# Data Professional Survey Breakdown


## Problem Statement

This breakdown helps with the better understanding of the professionals in the industry of data. It helps with the understanding of how satisfied an employee is with their jobs and how difficult/easy it was for them to step into the industry of Data. Furthermore, with different ratings and data collected in this real life survey, we can also gain some insights about important information like work life balance, payscale structure, average salary depending on the job title of the individuals, favorite programming language etc.


### Steps followed 

1. 

Opening the data to transform in the powerBI (Final_Project)


2. 

While working with the raw data, using 'Remove Column' to remove the unnecessary columns that we don't want to work with in our final visualization.


3. 

As the column 'Which title best fits your current position' has different kinds of data in different formats, to clean the
data, we need to perform the following:

Select the column > Select 'Split column' > 'Split column by delimiter' > Select 'Custom' in the first option > put '(' in the second blank space > Select 'Left most delimiter' in the 'Split at' option.

It should create another column with the extra data. We should remove that column.

NOTE: This step will make the filter a lot more simpler.


4. 

We will do the exact same steps for the column of 'Favorite Programming Language', as this column has a lot of
values that are subcategorized under the "Other:"

For this step, we will select the delimiter as the ':' and select the 'Left-most Delimiter' option.

Like previous step it will also create a separate column with the leftover data, that we will delete for our sorting
purposes.



5. 

We will be able to see that the salary column has a format of range.

To fix that we will do the following steps:

	1. We will make a duplicate of the salary column.

	2. In that duplicate column, we will again do the split column option, this time we will select the dropdown and select the 'Digit to non-digit option'.

	3. We will right click on the column header and select replace values. With this option we will delete the '-' 'k' that we can see in the range.



6. 

The whole point of the previous step is to create an average salary column. For that to work, we need to do the
following steps:

	1. Go to add column.

	2. Make sure that the data type in the columns that we just created in the previous steps are 'Whole numbers'

	3. Select the columns and divide them by 2. 

	(e.g. ([#"Q3 - Current Yearly Salary (in USD) - Copy.1"] + [#"Q3 - Current Yearly Salary (in USD) - Copy.2"]) / 2)

	4. Name the column. Make sure it does not detect any syntax error.



7. 

We will do the same split column method with the column for industry and country as well, where we want to sort out the 'Other: (' in the data.



### Visualization Steps:


        1. Adding a text box to add a title on the top.

        2. Adding card for both 'Unique ID' and 'Current Age'.

        3. A Stacked Bar chart based on Job title (X Axis) and Average Salary (Y Axis) with 'Job Title' as the legend.

                NOTE: We need to check wheter he average salary is in 'Decimal' data type or not, otherwise it will be difficult for the visualization.

        4. Treemap for countries. This will enable us to see the different values in the card when we select a particular part of it

        5. Guage: For guage we need a normal, a maximum and minimum value, (which we need to change after each selection with the right click).




### Visualization:

![Screenshot 2025-01-12 205648](https://github.com/user-attachments/assets/e3beb02b-73d0-4e4d-aa00-c1dd410d8942)

![Screenshot 2025-01-12 205723](https://github.com/user-attachments/assets/30c5a37b-b11e-4d05-ac81-1e08dae1434f)


![Screenshot 2025-01-12 210139](https://github.com/user-attachments/assets/742c9581-9172-4643-a799-49b0a88a2e25)

![Screenshot 2025-01-12 210236](https://github.com/user-attachments/assets/7b5879dd-5c8e-4192-b3b7-df1d0808fab1)

![Screenshot 2025-01-12 210331](https://github.com/user-attachments/assets/352949eb-07ac-4a30-9550-57448d36b8c0)

![Screenshot 2025-01-12 210439](https://github.com/user-attachments/assets/a1079ef7-4124-41e8-a507-ca764e19240d)

![Screenshot 2025-01-12 210514](https://github.com/user-attachments/assets/a835e618-ff45-42c9-8cd6-614d742b9571)
