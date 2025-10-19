# Sales-Dashboard
An interactive sales dashboard created using MS Excel that showcases sales of products of a cafe over the year of 2023.

1. Data:
     The data used in this project is of an cafe that is imaginary. This dataset is form Kraggle and these are not real and is
     made for public usage. This dataset contains sales data of a cafe for the year of 2023.
     This dataset contains over 10,000 rows and about 8 columns of dirty datas. This dataset has datas as follows, Transaction       ID, Item	Quantity,	Price Per Unit,	Total Spent,	Payment Method,	Location,	Transaction Date.
     The initial dataset is named dirty1.csv in this repositiry.
   
2. Data cleaning: 
     This dataset was cleaned using a combination of python.
     Steps taken to clean:
        1. imported pandas and numpy.
        2. Loaded the dirty dataset.
        3. Analyzed the dataset, found dirty datas like UNKNOWN, ERROR, and blanks in the dataset across multiple columns.
        4. Converted the UNKNOWN, ERROR, and blanks values into NaN across all the columns for easier cleaning.
        5. Replaced the NaN values in the Location with either 'in-store' or 'Takeaway' on random as there is no way to                  determine where the purchace happened. Similarly for the values in Payment method, NaN values has been replaced               between 'Cash','Credit card','Digital wallet'.
        6. For the columns - Quantity, Price Per Unit and Total Spent , we can calculate the missing values through simple               mathametics calculation.
        7. These values were calculated using these formulas,
                    Total Spent = Quantity * Price Per Unit
                    Quantity = Total Spent / Price Per Unit
                    Price Per Unit = Total Spent / Quantity
        8. Finally, filled the missing item names with respect to the price per item unit.
        9. Exported the cleaned csv file.








     
