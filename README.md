Problem 1
In a cricket tournament, based on the outcome of a particular match a team gets following points:
wins gets 7 points
draws gets 2 points
losses gets 0 points
Team Aravali plays 8 matches in this tournament. It wins 4 matches, loses 3 matches and draws 1. What is the total number of points gained by the Team aravali ?
a) The outcome variables are defined below?
b) Calculate the total points gained by Team Aravali and print.

Solution 1
wins = 4
draws = 1
losses = 3
total_points = (wins * 7) + (draws * 2) + (losses * 0)
print("Total points gained by Team Aravali:", total_points)


Problem 2
Root of a function  f(x)  is defined as the value  x  where  f(x)=0 
Consider a quadratic function  f(x)=x2+3x−4 
Find the value of the function  f(x)  at points  x=7,x=−1,x=1 .
  a)Calculate the value of the function f(x) at x = 2.
  b) Calculate the value of the function f(x) at x = 1

Solution 2
def f(x):
    return x**2 + 3*x - 4
print("f(7) =", f(7))
print("f(-1) =", f(-1))
print("f(1) =", f(1))
print("f(2) =", f(2))



Problem 3
A list contains the average daily temperature(in degree Celsius) of a city over a particular week. Write a Python code to swap the highest and the lowest temperatures
a) A list containing average daily temperature over a week 
temperatures = [34, 40, 29, 33, 42, 37, 39 ]
b) The expected output 
c)Store the highest temperature
d) Index of the element with the highest temperature
max_temp_index = 
e) Store the lowest temperature 
min_temp = 
f) Index of the element with the lowest temperature
min_temp_index = 

Solution 3
temperatures = [34, 40, 29, 33, 42, 37, 39]
max_temp = max(temperatures)
min_temp = min(temperatures)
max_temp_index = temperatures.index(max_temp)
min_temp_index = temperatures.index(min_temp)
temperatures[max_temp_index], temperatures[min_temp_index] = min_temp, max_temp

print("Temperatures after swapping highest and lowest values:", temperatures)

problem 4
Calculate the median price
a) Step 1 - Obtain the sorted list
b)Check if the number of elements in the list is even or odd
c)Use the corresponding formula to calculate the median and print the median
d) Check which is greater, mean or median

Solution 4
prices = [5, 9, 12, 11, 10]
sorted_prices = sorted(prices)
n = len(sorted_prices)
if n % 2 == 1:
    median = sorted_prices[n // 2] 
else:
    median = (sorted_prices[n // 2 - 1] + sorted_prices[n // 2]) / 2 
mean = sum(sorted_prices) / n
print("Median:", median)
print("Mean:", mean)
print("Median is greater than Mean:", median > mean)

Problem 5
Having a nested list sometimes might be a bit problematic. An individual was asked to collect the names of companies in the technology sector.
 While creating the list, by mistake the last three companies were subsumed in a list as shown below. You are required to get rid of the nesting
a)The list of tech companies curated by the individual
tech_companies = ['Qualcomm','Google','Apple',['Nvidia','Cisco','Samsung']]

Solution 5
tech_companies = ['Qualcomm', 'Google', 'Apple', ['Nvidia', 'Cisco', 'Samsung']]
flattened_tech_companies = tech_companies[:3] + tech_companies[3]
print("Flattened tech companies list:", flattened_tech_companies)

Problem 6
Another measure of average
Mode is defined as the value that appears most often in a set of data values. Mode corresponds to the most frequent value.
You are given a list of numbers and you need to calculate the mode of this list.
A list containing average daily temperature over 10 days
temperatures = [34, 40, 29, 33, 42, 40, 39, 34, 34,33 ]

Solution 6
from collections import Counter
temperatures = [34, 40, 29, 33, 42, 40, 39, 34, 34, 33]
frequency = Counter(temperatures)
mode = max(frequency, key=frequency.get)
print("Mode of the temperatures:", mode)


