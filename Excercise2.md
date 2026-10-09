
START

Set highest average = 0
Set lowest average = 100

FOR student = 1 TO 5

    INPUT mark1
    INPUT mark2
    INPUT mark3
    INPUT mark4
    INPUT mark5

    IF any mark is missing OR any mark is less than 0 OR greater than 100 THEN

        DISPLAY "Student did not sit for the exam"

    ELSE

        Set sum = mark1 + mark2 + mark3 + mark4 + mark5

        Set average = sum / 5

        IF average >= 90 THEN
            Set grade = "A"

        ELSE IF average >= 80 THEN
            Set grade = "B"

        ELSE IF average >= 70 THEN
            Set grade = "C"

        ELSE IF average >= 60 THEN
            Set grade = "D"

        ELSE IF average >= 50 THEN
            Set grade = "E"

        ELSE
            Set grade = "F"
        END IF

        DISPLAY average
        DISPLAY grade

        IF average > highest average THEN
            Set highest average = average
        END IF

        IF average < lowest average THEN
            Set lowest average = average
        END IF

    END IF

END FOR

DISPLAY "Highest average is ", highest average
DISPLAY "Lowest average is ", lowest average

END