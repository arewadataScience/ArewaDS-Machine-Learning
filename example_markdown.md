import pandas as pd

# Load the data from the uploaded file
file_path = '/path/to/your/file.csv'  # Replace with your file path
data = pd.read_csv(file_path)

# Group the data by 'Name (Original Name)' and sum the 'Duration (Minutes)'
grouped_data = data.groupby('Name (Original Name)')['Duration (Minutes)'].sum().reset_index()

# Rename the columns for clarity
grouped_data.columns = ['Name', 'Total Duration (Minutes)']

# Save the aggregated data to a new CSV file
output_file_path = '/path/to/save/aggregated_data.csv'  # Replace with your desired file path
grouped_data.to_csv(output_file_path, index=False)
