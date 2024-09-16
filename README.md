import numpy as np



n = int(input("Enter how many categories of grading are there that you have? (Enter it as a number)"))

grade_percent =  np.array([])
grade_points = np.array([])
for i in range(0 , n):
    percent = int(input("What percent do you have in this category "))
    grade_percent = np.append(grade_percent, percent)
    points = int(input("How many points is this category worth?"))
    grade_points = np.append(grade_points , points)
tot_points = np.array((grade_percent * .01) * grade_points)
print(np.sum(tot_points))
