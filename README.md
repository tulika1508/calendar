# Calendar Program

This is a simple C program to generate and print the calendar for a given year. The program takes a year as input and displays the calendar for that year, month by month.

## Files

- `calendar.c`: Contains the main code for generating and printing the calendar.

## Compilation

To compile the program, use a C compiler like `gcc`. Run the following command in the terminal:

```sh
gcc -o calendar calendar.c
```

This command will compile the source code and create an executable file named `calendar`.

## Usage

After compiling the program, run the executable file:

```sh
./calendar
```

The program will prompt you to enter a year. After entering the year, the program will print the calendar for that year.

## Functions

### `int dayNumber(int day, int month, int year)`

Calculates the day of the week for a given date. The return value is an integer representing the day of the week (0 for Sunday, 1 for Monday, ..., 6 for Saturday).

### `char* getMonthName(int monthNumber)`

Returns the name of the month for a given month number (0 for January, 1 for February, ..., 11 for December).

### `int numberOfDays(int monthNumber, int year)`

Returns the number of days in a given month of a specified year. It accounts for leap years when determining the number of days in February.

### `void printCalendar(int year)`

Prints the calendar for the entire year month by month. Each month is printed with the days of the week properly aligned.

## Example

```
Enter the year:
2024
    Calendar - 2024

 ------------January-------------
 Sun    Mon    Tue    Wed    Thu    Fri    Sat
        1      2      3      4      5      6
  7      8      9     10     11     12     13
 14     15     16     17     18     19     20
 21     22     23     24     25     26     27
 28     29     30     31

 ------------February-------------
 Sun    Mon    Tue    Wed    Thu    Fri    Sat
                          1      2      3
  4      5      6      7      8      9     10
 11     12     13     14     15     16     17
 18     19     20     21     22     23     24
 25     26     27     28     29

...

 ------------December-------------
 Sun    Mon    Tue    Wed    Thu    Fri    Sat
  1      2      3      4      5      6      7
  8      9     10     11     12     13     14
 15     16     17     18     19     20     21
 22     23     24     25     26     27     28
 29     30     31
```

## Notes

- The program correctly accounts for leap years.
- The output is formatted with each month displayed in a grid layout showing the days of the week.
