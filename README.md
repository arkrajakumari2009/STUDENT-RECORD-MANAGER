# STUDENT-RECORD-MANAGER

A small command-line project for managing student records. It is designed as a first C project and practices `struct`, arrays, functions, loops, and file handling.

## Features

- Add a student with a unique roll number, name, and marks
- List all saved students
- Search by roll number
- Update a student's name or marks
- Delete a student record
- Keep records between runs in `students.dat`

## Build and run

You need a C compiler such as GCC.

### Windows (MinGW GCC)

Open PowerShell or Command Prompt in this folder:

```text
gcc student_records.c -o student_records.exe
student_records.exe
```

### macOS or Linux

```text
gcc student_records.c -o student_records
./student_records
```

The program creates `students.dat` in its current working folder the first time it saves records. Keep that file if you want your records next time; delete it to start with an empty list.

## Menu

```text
1. Add student
2. List students
3. Search by roll number
4. Update student
5. Delete student
0. Save and exit
```

## Notes

- This learning project stores up to 100 records.
- The data file is a simple binary file intended for this program, not a portable export format such as CSV.
- Do not put private or real student information in a public GitHub repository. The generated `students.dat` is local data and should not be committed.

## Possible improvements

- Export records as CSV
- Add sorting by marks or name
- Calculate class average and highest marks
- Add input validation for names with longer than 49 characters
