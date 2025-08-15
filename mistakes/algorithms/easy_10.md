```python
def gradingStudents(grades):
    round_grades = []
    for grade in grades:
        if grade < 38:
            round_grades.append(grade)
        else:
            a = ((grade // 5) + 1) * 5
            b = a - grade
            if b < 3:
                round_grades.append(a)
            else:
                round_grades.append(grade)
    return round_grades
```

Convert each grade into a better one.
1. Create an empty list to store the rounded grades.
2. Iterate over the original grades.
3. If a grade is less than 38, append it unchanged.
4. For grades whose last digit is 3,4, 8 or 9 (e.g., 43, 44, 48, 49, 58, 59), take the floor after dividing by 5, add 1, then multiply by 5 to get the rounded grade.
43,44-->45  48,49-->50
5. For grades ending in 5, 6, or 7 (e.g., 45, 46, 47), simply append the original grade.
45,46,47-->45,46,47

**time complexity** :O(g)g = len(grades)
**space complexity** :O(g)