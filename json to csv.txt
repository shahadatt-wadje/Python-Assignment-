# Program 2: Convert JSON array into CSV file

import json
import csv

# Open and read the JSON file
with open('data.json', 'r') as json_file:
    data = json.load(json_file)

# Open CSV file for writing
with open('data.csv', 'w', newline='') as csv_file:

    # Get field names (keys from first JSON object)
    fieldnames = data[0].keys()

    writer = csv.DictWriter(csv_file, fieldnames=fieldnames)

    # Write header
    writer.writeheader()

    # Write rows
    writer.writerows(data)

print("JSON data successfully converted to CSV.")
