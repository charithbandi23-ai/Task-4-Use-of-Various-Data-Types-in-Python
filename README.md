4.1 Student Marks Average

Scenario: To create an empty list to store student records (name and marks). Input the number of students. For each student, input name and marks and append the record to the list. Calculate the total marks and compute the average. Iterate through the list and if a student's marks are greater than the average, display them.

Algorithm:

1. Create an empty list to store student records.

2. Input number of students.

3. For each student, input name and marks and append the record to the list.

4. Calculate total marks and compute average marks.

5. Iterate through the list and display students with marks greater than average.

Code:
num_students = int(input("Enter the number of students: "))
Students = []
for i in range(num_students):
    name = input(f"Enter name of student {i+1}: ")
    marks = float(input(f"Enter marks of student {i+1}: "))
    Students.append((name, marks))
total_marks = sum(marks for name, marks in Students)
average_marks = total_marks / num_students
print(f"Average marks: {average_marks}")
print("Students who scored above average:")
for name, marks in Students:
    if marks > average_marks:
        print(f"{name} - {marks}")
   
Output:
Average marks: 78.71428571428571
Students who scored above average: 85, 90, 92, 81
