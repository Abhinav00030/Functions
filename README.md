# List to store student information
students = []

def student_info():
    """
    Collect and store information for a single student.
    
    This function prompts the user for student ID, name, and phone number,
    then stores this information as a dictionary in the global 'students' list.
    """
# Collect student information from user input
    Student_id = input('Enter student ID: ')
    student_name = input('Enter student name: ')
    student_phone = input('Enter student phone number: ')
    
# Create a dictionary to store the student's information
    entry = {
        'Student ID': Student_id,
        'Student Name': student_name,
        'Student Phone': student_phone,
    }

# Add the student entry to the list of students
    students.append(entry)

def print_entries():
    """
    Print all stored student entries.
    
    This function iterates through the 'students' list and prints
    each student's information in a formatted string.
    """
    print('\nAll student entries:')
    for entry in students:
        print(f"ID: {entry['Student ID']}, Name: {entry['Student Name']}, Phone: {entry['Student Phone']}")

# Note: To use these functions, call student_info() to add a new student,
# and print_entries() to display all stored student information.
