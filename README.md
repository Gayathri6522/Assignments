import numpy as np
import pandas as pd

# Create a NumPy array from 1 to 10 and reshape it to 2x5
arr1 = np.arange(1, 11)
matrix = arr1.reshape(2, 5)

print("Question 1:")
print(matrix)

# Create a NumPy array from 1 to 10 and reshape it to 2x5
arr1 = np.arange(1, 11)
matrix = arr1.reshape(2, 5)

print("Question 1:")
print(matrix)

# Compute mean, median, and standard deviation
mean = np.mean(arr2)
median = np.median(arr2)
std = np.std(arr2)

print("\nQuestion 3:")
print("Mean =", mean)
print("Median =", median)
print("Standard Deviation =", std)

# Broadcasting
x = np.array([[1, 2, 3, 4],
              [5, 6, 7, 8],
              [9, 10, 11, 12]])

y = np.array([1, 2, 3, 4])

result = x - y

print("\nQuestion 4:")
print("Array X:")
print(x)
print("Array Y:")
print(y)
print("Result after broadcasting:")
print(result)

# Create DataFrame
data = {
    "name": ["Alice", "Bob", "Charlie", "David", "Emma",
             "Frank", "Grace", "Henry", "Isabella", "Jack"],
    "age": [25, 30, 28, 35, 40, 22, 31, 29, 45, 33],
    "gender": ["Female", "Male", "Male", "Male", "Female",
               "Male", "Female", "Male", "Female", "Male"]
}

df = pd.DataFrame(data)

print("\nQuestion 5:")
print(df)

# Add Occupation column
occupations = ["Programmer", "Manager", "Analyst",
               "Programmer", "Manager", "Analyst",
               "Programmer", "Manager", "Analyst",
               "Programmer"]

df["occupation"] = occupations

print("\nDataFrame after adding Occupation:")
print(df)

# Select rows where age >= 30
age_30 = df[df["age"] >= 30]

print("\nRows where age >= 30:")
print(age_30)

# Convert DataFrame to CSV 
df.to_csv("people.csv", index=False)

new_df = pd.read_csv("people.csv")

print("\nContents of CSV File:")
print(new_df)
