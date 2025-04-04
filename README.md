# Student Information Management Using YAML

## Overview
This Python application reads student information from a YAML file and provides options to display all students and filter them based on their GPA.

## Features
- Load student data from a YAML file.
- Display all students with their details.
- Filter students based on a minimum GPA input by the user.

## Prerequisites
Ensure you have Python installed on your system. Additionally, you need the `PyYAML` library to handle YAML files. You can install it using:

```bash
pip install pyyaml
```

## Project Structure
```
student_management/
│-- app.py
│-- students.yaml
│-- README.md
```

## YAML File Structure
Create a `students.yaml` file with the following format:

```yaml
students:
  - name: Alice
    age: 21
    major: Computer Science
    gpa: 3.8
  - name: Bob
    age: 22
    major: Mathematics
    gpa: 3.5
  - name: Charlie
    age: 20
    major: Physics
    gpa: 3.9
  - name: David
    age: 23
    major: Chemistry
    gpa: 3.2
  - name: Eva
    age: 21
    major: Computer Science
    gpa: 3.7
```

## Usage

1. Clone the repository or create the required files in a directory.
2. Ensure the `students.yaml` file is in the same directory as `app.py`.
3. Run the Python script:
   
   ```bash
   python app.py
   ```
4. The script will display all students and prompt you to enter a minimum GPA for filtering.

## Expected Output
```
All Students:
Name: Alice, Age: 21, Major: Computer Science, GPA: 3.8
Name: Bob, Age: 22, Major: Mathematics, GPA: 3.5
Name: Charlie, Age: 20, Major: Physics, GPA: 3.9
Name: David, Age: 23, Major: Chemistry, GPA: 3.2
Name: Eva, Age: 21, Major: Computer Science, GPA: 3.7

Enter minimum GPA to filter students: 3.6
Students with GPA >= 3.6:
Name: Alice, Age: 21, Major: Computer Science, GPA: 3.8
Name: Charlie, Age: 20, Major: Physics, GPA: 3.9
Name: Eva, Age: 21, Major: Computer Science, GPA: 3.7
```

## Explanation
- **`load_data(file_path)`**: Reads data from the YAML file.
- **`display_students(students)`**: Displays all students' details.
- **`filter_students_by_gpa(students, min_gpa)`**: Filters students with a GPA above the specified value.
- **`main()`**: Manages the execution flow of the program.

## Future Enhancements
- Add functionality to update student records.
- Allow users to save filtered data to a new YAML file.
- Implement sorting features based on different attributes.

## License
This project is open-source and available for modification and redistribution.



