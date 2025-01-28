# Advanced-Sales-Analytics-and-Customer-Segmentation
 ## Project Description
This project focuses on uncovering customer patterns through advanced sales analytics and segmentation techniques. By leveraging machine learning models and demographic attributes, we aim to provide actionable insights to enhance strategic decision-making in sales and marketing.

## Dataset Description
The dataset originates from the UCI Machine Learning Repository, containing real transaction data from a UK-based online retail company. It spans from December 1, 2010, to December 9, 2011, with 541,910 rows and attributes such as:

- `InvoiceNo`: Unique invoice number  
- `StockCode`: Product code  
- `Description`: Product description  
- `Quantity`: Items purchased  
- `InvoiceDate`: Purchase date  
- `UnitPrice`: Price per unit  
- `CustomerID`: Unique customer identifier  
- `Country`: Customer's location  

This dataset provides comprehensive insights into the operations of an online retailer, including sales trends and customer behaviors.

## Analysis Steps
### Step 1: Data Preprocessing
```python
# Example of handling missing values
data = data.dropna(subset=["CustomerID", "Description"])
data["TotalPrice"] = data["Quantity"] * data["UnitPrice"]
