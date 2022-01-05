# DataClasses_WideWorldImporters

This repository contains CSV files exported via SQL queries from Azure Data Studio. THe data is gathered from the Wide World Importers database; more specifically, the Sales.Orders, Sales.Invoices, and the Sales.Customers tables. The dataclasses created for these did not include all columns from those tables. Only the columns that seemed to consistently have relevant information (i.e. infrequently had NULL values) were chosen.

Any ID attributes or any variable representing a quantity of some sort will need to be converted to integers using the int() method. Any columns with 'date' in their headers will need their values converted to date objects by using the datetime.datetime.date() method. The discount percentage variable in Sales.Customer will also need to be converted to a float type using the float() method.
