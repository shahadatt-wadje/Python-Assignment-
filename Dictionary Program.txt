# 1. Create and Access Dictionary Elements
print("1. Create and Access Dictionary Elements")

student = {
    "roll_no": 101,
    "name": "Amit",
    "marks": 85
}

print("Dictionary:", student)
print("Name:", student["name"])
print("Marks:", student.get("marks"))
print()


# 2. Update Dictionary
print("2. Update Dictionary")

student["marks"] = 90          # Update existing value
student["grade"] = "A"         # Add new key-value pair

print("Updated Dictionary:", student)
print()


# 3. Removing Elements
print("3. Removing Elements")

removed_value = student.pop("grade")   # Remove specific key
print("Removed Value:", removed_value)
print("After Removing 'grade':", student)

student.popitem()   # Removes last inserted item
print("After popitem():", student)
print()


# 4. Merging Dictionaries
print("4. Merging Dictionaries")

dict1 = {"a": 1, "b": 2}
dict2 = {"c": 3, "d": 4}

# Method 1 (Python 3.9+)
merged_dict = dict1 | dict2

# Method 2 (Works in all Python versions)
# merged_dict = dict1.copy()
# merged_dict.update(dict2)

print("First Dictionary:", dict1)
print("Second Dictionary:", dict2)
print("Merged Dictionary:", merged_dict)
