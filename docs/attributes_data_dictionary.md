import pandas as pd

# Get the list of column names in the df_squad dataframe
column_names = df_squad.columns.tolist()

# Create an empty dictionary to store the column descriptions
data_dictionary = {}

# Iterate over each column name
for column_name in column_names:
    # Provide a description for each column
    if column_name == 'column1':
        description = 'Description of column1'
    elif column_name == 'column2':
        description = 'Description of column2'
    # Add the description to the dictionary
    data_dictionary[column_name] = description

# Create a DataFrame from the data dictionary
df_data_dictionary = pd.DataFrame(data_dictionary.items(), columns=['Column Name', 'Description'])

# Display the data dictionary table
print(df_data_dictionary)

