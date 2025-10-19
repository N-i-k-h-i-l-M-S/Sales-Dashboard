An interactive sales dashboard created using MS Excel that showcases sales of products of a cafe over the year of 2023.

Data:
The data used in this project is of a cafe that is imaginary. This dataset is from Kaggle and these are not real and are made for public usage. This dataset contains sales data of a cafe for the year of 2023.
This dataset contains over 10,000 rows and about 8 columns of dirty data. This dataset has data as follows: Transaction ID, Item, Quantity, Price Per Unit, Total Spent, Payment Method, Location, Transaction Date.
The initial dataset is named dirty1.csv in this repository.

Data cleaning:
This dataset was cleaned using a combination of Python.
Steps taken to clean:

1. Imported pandas and numpy.

2.Loaded the dirty dataset.

3. Analyzed the dataset, found dirty data like UNKNOWN, ERROR, and blanks in the dataset across multiple columns.

4. Converted the UNKNOWN, ERROR, and blank values into NaN across all the columns for easier cleaning.

5. Replaced the NaN values in the Location with either 'In-store' or 'Takeaway' randomly as there is no way to determine where the purchase happened. Similarly, for the values in Payment Method, NaN values have been replaced with 'Cash', 'Credit card', or 'Digital wallet'.

6. For the columns - Quantity, Price Per Unit, and Total Spent, we can calculate the missing values through simple mathematical calculations.

These values were calculated using these formulas:

Total Spent = Quantity × Price Per Unit

Quantity = Total Spent ÷ Price Per Unit

Price Per Unit = Total Spent ÷ Quantity

7. Finally, filled the missing item names with respect to the price per item unit.

8. Exported the cleaned CSV file.

Dashboard:
This interactive dashboard is made using MS Excel. With the help of Pivot Tables, I made graphs and other visual representations of the data. This dashboard shows many data comparisons between various items sold in the cafe. It also shows the comparison between the payment methods used by people to purchase. It also showcases the month-by-month sales of each item in the cafe. All these comparisons have visual charts to easily see and understand the data. The dashboard also includes a slicer for the items that allows viewing individual sales data of products. It also has a timeline slicer that allows viewing sales of the cafe for individual months.

Future usage:
As this dashboard is made using Pivot Tables, it's easy to update the data for the future. The future data just needs to be added to the data page of the Excel file, and the dashboard will automatically update.

Thank you for reading and accessing this project. If you have any queries or tips for improving this project, let me know :)
Again, thank you.
