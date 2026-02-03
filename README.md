# Ex.No: 01A PLOT A TIME SERIES DATA
###  Date: 3/02/2026
# Name : Ramasri K
# Reg No: 212224040267

# AIM:
To Develop a python program to Plot a time series data (population/ market price of a commodity
/temperature.
# SOFTWARE REQUIRED:
Google Colab
# ALGORITHM:
1. Import the required packages like pandas and matplot
2. Read the dataset using the pandas
3. Calculate the mean for the respective column.
4. Plot the data according to need and can be altered monthly, or yearly.
5. Display the graph.
# PROGRAM:
```
import pandas as pd
import matplotlib.pyplot as plt
df=pd.read_csv('/content/silver_prices_data.csv')
df.info()
df = df.sort_values('Date')
plt.plot(df['Date'], df['Volume'], marker='o')
plt.xlabel("Date")
plt.ylabel("Volume")
plt.title("Volume over Date")
plt.grid(True)
plt.show()
df['Date'] = pd.to_datetime(df['Date'])
df = df.sort_values('Date')
plt.plot(df['Date'], df['Volume'])
plt.xlabel("Date")
plt.ylabel("Volume")
plt.title("Volume over Date")
plt.grid(True)
plt.show()
```
# OUTPUT:

<img width="1552" height="93" alt="image" src="https://github.com/user-attachments/assets/d0add89f-5208-4c1f-a3be-fdd5e6934cec" />
<img width="1486" height="534" alt="image" src="https://github.com/user-attachments/assets/1142a8ce-8018-4c91-8b06-7ecff4483607" />
<img width="1186" height="557" alt="image" src="https://github.com/user-attachments/assets/1acbe622-6d4d-4b96-b4fb-c432936251a9" />
<img width="1146" height="81" alt="image" src="https://github.com/user-attachments/assets/34044124-b604-4ca9-baed-f7040b4fe46c" />
<img width="1787" height="724" alt="image" src="https://github.com/user-attachments/assets/c110ece4-3b37-4302-b648-5f5e817b9235" />

# RESULT:
Thus we have created the python code for plotting the time series of given data.
