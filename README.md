# Lab-11

Write a program that outputs the day of the week for a given date. Your program should have two methods:  the main method and the dayOfWeek method described below.  


Requirements-
-	Your typical header, including your name, date, project title and project description must be included.
-	Programming comments should be included for each logical block of code.
-	Program should ask the user to enter a date in the format of month/date/year (##/##/####)
-	After the user enters a date, the program should identify which digits correspond to month (int), day (int) and year(int).
-	The program should pass the values to the method dayOfWeek as specified in the header below. Include comments before the method describing the method, the parameters and return value.  (As shown below)

```
    //dayOfWeek method – given a date, returns the day of week
    //precondition:  int m(month), int d (day), int y (year)
    //postcondition:  returns the day of the week (String)

    public static String dayOfWeek(int m, int d, int y)
    {
    	// fill in code
    }
```
-	The method should return a String that contains the day of the Week for that date using the formulas below:

Given the month, m, day, d and year y, the day of the week(Sunday = 0, Monday = 1, …, Saturday = 6).   D is given by:
```math
y_0 = y - (14 - m)/12
```
```math
x_0 = y_0 + y_0 / 4 - y_0 / 100 + y_0 / 400
```
```math
m_0 = m + 12 \times ((14 - m) / 12) - 2
```
```math
D = (d + x_0 + 31 \times m_0 / 12)  \mod\  7
```
<br />
Note: the division above is integer division. mod is the % operator.

The day of the week output should occur within the main method.  Output should be easy to read, with no typographical errors.

    Output:
        Enter a date in the format month/day/year (##/##/####)  10/15/2019
        Day of the week: Tuesday


Be sure to use conditionals! Be sure to test with many different dates.  Try entering your birthday and test your parents’ birthdays!
