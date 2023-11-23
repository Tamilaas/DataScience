import pandas as pd
import numpy as np
data = {
    'Temperature': [20, 25, 18, 22, 19],
    'Humidity': [50, 60, 45, 55, 52],
    'Pressure': [1013, 1010, 1015, 1008, 1012]
}
weather_data = pd.DataFrame(data)
std_temperature = np.std(weather_data['Temperature'])
std_humidity = np.std(weather_data['Humidity'])
std_pressure = np.std(weather_data['Pressure'])

print("Стандартное отклонение для столбца 'Temperature':", std_temperature)
print("Стандартное отклонение для столбца 'Humidity':", std_humidity)
print("Стандартное отклонение для столбца 'Pressure':", std_pressure)


import pandas as pd
data = {
    'Name': ['Аружан', 'Дамир', 'Айым', 'Темирлан', 'Молдир'],
    'Age': [28, 35, 30, 32, 29],
    'Salary': [50000, 60000, 55000, 62000, 52000],
    'Education': ['Bachelor', 'Master', 'Bachelor', 'PhD', 'Master']
}
employee_data = pd.DataFrame(data)
print(employee_data.describe())


import pandas as pd
import numpy as np
data = {
    'Name': ['John', 'Emily', 'Michael', 'Sophia', 'William'],
    'Height': [170, 165, 180, 155, 175],
    'Income': [50000, 60000, 55000, 62000, 52000],
    'Age': [30, 28, 35, 25, 32]
}
people_data = pd.DataFrame(data)
income = people_data["Income"]
percentile25 = np.percentile(income, 25)
percentile50 = np.percentile(income, 50)
percentile75 = np.percentile(income, 75)
print("25-й процентиль:", percentile25)
print("50-й процентиль:", percentile50)
print("75-й процентиль:", percentile75)




