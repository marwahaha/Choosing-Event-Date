# Choosing-Event-Date
A python console application to easily see which dates most people are free on to help with event planning.

Please Note: This is very very buggy :(...

### Installing and Running the Programme
**Files Needed**
1. Main.py
2. human_in.txt

**Instructions**
+ Fill in information on dates which have people unavailable into human_in.txt (format below).
+ Run main.py.

**Formatting**
1. A datetime is the combination of a date and a time.
2. All datetimes are in the format (day month year hour:min am/pm) where month is the 3 letter abbreviation for each month (E.g. '14 nov 2018 12:00 pm').
3. The first line contains 2 datetimes, *s* and *e*. *s* is the earliest date time possible to start the even.*e* is the latest possible time to end the event. 
4. The time of *s* and the time of *e* are the earliest and latest times the event being planned can start or end.
4. The second line contains abbreviations of days of the week (first 3 letters of each day). These days indicate days of the week which are to be blocked off. E.g. writing 'sun mon' would block sundays and mondays from appearing in the results.
5. The next (as many as you like) lines each consist of 2 datetimes (e.g. '3 dec 2018 12:00 am 11 dec 2018 11:00 pm'). These would be the start and end datetimes a person would not be able to attend the event being planned.
6. The last line is a 'break' to signal for the program to stop reading the file.

Example:<pre>
14 nov 2018 8:00 am 31 dec 2018 10:00 pm
mon tue wed thurs fri
24 nov 2018 12:00 am 2 dec 2018 11:00 pm
20 dec 2018 12:00 am 26 dec 2018 11:00 pm
5 dec 2018 12:00 am 12 dec 2018 11:00 pm
10 dec 2018 12:00 am 25 dec 2018 11:00 pm
24 nov 2018 12:00 am 6 dec 2018 11:00 pm
3 dec 2018 12:00 am 11 dec 2018 11:00 pm
18 nov 2018 12:00 am 18 nov 2018 11:00 pm
17 nov 2018 1:00 pm 17 nov 2018 5:00 pm
break
</pre>

In this example, 
1. The event is only allowed to be between 14th of nov to the 31th of december. 
2. The event is only allowed to be between 8 am to 10 pm each day.
3. The event is only allowed to occur on weekends.

Larger Example
<pre>
12 nov 2018 4:00 pm 16 nov 2018 11:59 pm

12 nov 2018 1:00 pm 12 nov 2018 4:00 pm
14 nov 2018 3:00 pm 14 nov 2018 6:00 pm
16 nov 2018 1:00 pm 16 nov 2018 4:00 pm

13 nov 2018 5:30 pm 13 nov 2018 7:30 pm
14 nov 2018 5:30 pm 14 nov 2018 7:30 pm
15 nov 2018 5:30 pm 15 nov 2018 7:30 pm
16 nov 2018 5:30 pm 16 nov 2018 7:30 pm

12 nov 2018 9:00 am 12 nov 2018 11:00 am
14 nov 2018 2:00 pm 14 nov 2018 5:00 pm
16 nov 2018 2:00 pm 16 nov 2018 5:00 pm

12 nov 2018 9:00 am 12 nov 2018 4:30 pm
14 nov 2018 2:00 pm 14 nov 2018 5:00 pm

14 nov 2018 3:00 pm 14 nov 2018 5:00 pm
16 nov 2018 3:00 pm 16 nov 2018 5:00 pm

13 nov 2018 3:30 pm 13 nov 2018 6:30 pm
16 nov 2018 3:30 pm 16 nov 2018 6:30 pm

14 nov 2018 3:00 pm 14 nov 2018 5:00 pm
15 nov 2018 9:00 am 15 nov 2018 11:00 am
break
</pre>
