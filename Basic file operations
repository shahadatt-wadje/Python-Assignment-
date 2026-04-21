#Open a file in write mode and write data
with open("sample.txt", "w") as file:
    file.write("Hello, this is the first line in the file.\n")
    file.write("File handling in Python is easy to learn.\n")

print("Data written successfully.\n")

#Open the file in read mode and display contents
with open("sample.txt", "r") as file:
    print("Reading file contents:")
    content = file.read()
    print(content)

#Open the file in append mode and add more data
with open("sample.txt", "a") as file:
    file.write("This line is added using append mode.\n")

print("\nData appended successfully.\n")

#Read the file again to see updated content
with open("sample.txt", "r") as file:
    print("Updated file contents:")
    print(file.read())
