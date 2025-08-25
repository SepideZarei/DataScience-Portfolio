python
>>> import pandas as pd
>>> import matplotlib.pyplot as plt
>>> data = {
...     "City": ["Tehran", "Shiraz", "Tabriz", "Isfahan", "Rasht"],
...     "Temperature": [32, 36, 29, 34, 28],
...     "Rainfall": [2, 0, 5, 1, 20]
... }
>>> df = pd.DataFrame(data)
>>> print("Weather dataset:\n")
Weather dataset:

>>> print(df)
      City  Temperature  Rainfall
0   Tehran           32         2
1   Shiraz           36         0
2   Tabriz           29         5
3  Isfahan           34         1
4    Rasht           28        20
>>> print("\nAverage Temperature:", df["Temperature"].mean())

Average Temperature: 31.8
>>> print("Average Rainfall:", df["Rainfall"].mean())
Average Rainfall: 5.6
>>> plt.figure(figsize=(8,5))
<Figure size 800x500 with 0 Axes>
>>> plt.bar(df["City"], df["Temperature"], color="orange")
<BarContainer object of 5 artists>
>>> plt.title("Average Temperature in Cities")
Text(0.5, 1.0, 'Average Temperature in Cities')
>>> plt.xlabel("City")
Text(0.5, 0, 'City')
>>> plt.ylabel("Temperature (C)")
Text(0, 0.5, 'Temperature (C)')
>>> plt.show()
>>>
>>>
>>> plt.xlabel("City")
Text(0.5, 0, 'City')
>>>
>>> plt.figure(figsize=(8,5))
<Figure size 800x500 with 0 Axes>
>>> plt.bar(df["City"], df["Rainfall"], color="blue")
<BarContainer object of 5 artists>
>>> plt.title("Rainfall in Cities")
Text(0.5, 1.0, 'Rainfall in Cities')
>>> plt.xlabel("City")
Text(0.5, 0, 'City')
>>> plt.ylabel("Rainfall (mm)")
Text(0, 0.5, 'Rainfall (mm)')
>>> plt.show()