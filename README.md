Aim:

To analyze quarterly sales data using NumPy arrays.

Algorithm:
1. Import NumPy.
2. Create 2D array (rows = products, columns = quarters).
3. Calculate total and average sales per product and per quarter.
4. Display summary.
Program:
import numpy as np

sales = np.array([[1000, 1200, 1150, 1400],
                  [800, 950, 1050, 1300],
                  [1500, 1600, 1550, 1700]])

print("Sales Data (Rows=Products, Columns=Quarters):\n", sales)

product_total = np.sum(sales, axis=1)

quarter_total = np.sum(sales, axis=0)

overall_avg = np.mean(sales)

print("\nTotal Sales per Product:", product_total)

print("Total Sales per Quarter:", quarter_total)

print("Overall Average Sales:", overall_avg)

print("Highest Sale:", np.max(sales))

print("Lowest Sale:", np.min(sales))

output

<img width="450" height="212" alt="image" src="https://github.com/user-attachments/assets/1205fffc-3185-4133-91bd-c91bf4a3638c" />

Result:
The program successfully analyzes quarterly product sales using NumPy arrays and Python functions.
