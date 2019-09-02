# Ex.
# Create a function that takes a nested list as a argument
# and a search value and returns the ocurrences of an item
nested_list = [[1,2,3],[6,7,6],[1,6,3]]
# nested_occurrences(nested_list,6) ----> 3

# Hint: use nested for loops

def nested_occurrences(a_list, a_number):
    counter = 0
    for every_list in a_list:
        for element in every_list:
            if element==a_number:
                counter += 1
    return counter

def nested_occurrences_indexes(a_list, a_number):
    counter = 0
    for row_index in range(len(a_list)): # [0,1,2,3]
        for col_index in range(len(a_list[row_index])):
            if a_list[row_index][col_index]==a_number:
                counter += 1
    return counter

print(nested_occurrences(nested_list,6))
print(nested_occurrences_indexes(nested_list,6))



# Ex.2
# Create a function that takes number of rows and number of
# columns and returns a nested list with of that size
# with all elements = 0

# create_nested(2,3) --> [[0,0,0],[0,0,0]]
# create_nested(3,3) --> [[0,0,0],[0,0,0],[0,0,0]]

def new_nested_list(rows, cols):
    nested_list = []
    for each_row in range(rows):
        new_row=[]
        for each_col in range(cols):
            new_row.append("0")
        nested_list.append(new_row)
    return nested_list

print(new_nested_list(2,3))
