# CSV Cleaner 🧹

A Python program that cleans and reformats student data from a CSV file.

## About the Project
The program reads a CSV file containing student names and their Hogwarts houses. The original file stores the student's first and last name together in one column.

The program separates the name into **first name** and **last name**, then writes the cleaned data to a new CSV file.

For example:

```text
"Abbott, Hannah",Hufflepuff
```

is converted to:

```text
Hannah,Abbott,Hufflepuff
```

## How It Works

The program takes two command-line arguments:

1. The name of the input CSV file
2. The name of the output CSV file

Example:

```bash
python scourgify.py before.csv after.csv
```

The output file contains three columns:

```text
first,last,house
```

The program also handles invalid command-line arguments and files that cannot be read.

## Error Handling

The program exits with an error message when:

* No input and output files are provided
* More than two command-line arguments are provided
* The input file cannot be read

Example:

```text
Too few command-line arguments
```

```text
Too many command-line arguments
```

```text
Could not read before.csv
```

## What I Practiced

* Command-line arguments
* `sys.argv`
* `sys.exit()`
* Reading CSV files
* Writing CSV files
* `csv.DictReader`
* `csv.DictWriter`
* Dictionary data
* String manipulation
* Splitting names
* File handling
* Error handling with `try` and `except`

## Technologies

* Python
* CSV

## Course

This project was completed as part of **CS50's Introduction to Programming with Python** by Harvard University.
