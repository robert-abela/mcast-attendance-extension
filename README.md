# MCAST Attendance Helper v0.7.1

**Note: This Chrome extension is no longer usable since the website it was meant to enhance has been shut down. The repository is kept online for pure reference**

A chrome extension that assists MCAST lecturers in filling their attendance. Works in basic mode by default and in advanced mode if configured.

## Basic Mode
Adds a new button that when pressed counts the number or students marked as present. Also makes some class list headers clickable to set all students present or absent.
Activates only when visiting https://attendance.mcast.edu.mt to **Add or Edit Attendance** entries. 

## Advanced Mode
Advanced Mode: Adds Autofill and Remember functionalities. 

**Autofill** Attendance is a link that automatically fills Class, Unit, Session & Duration fields if the attendance is being added during the lesson (day of the week and time need to match). Activates when the user has configured the timetable in Options. 

**Remember** allows the lecturer to save the state of attendance (Absent/Present, Reason & Remark for each student) and to automatically set them again thereafter.

Timetable configured with CSV rows, each line represents a lesson and is in the format: DDD,CLASS,START,END,UNIT as detailed below:

* DDD: 3 letter day of the week, e.g.: Mon, Thu
* CLASS: class name, e.g.: IT-SWD-6.2A
* START,END: 24-hr clock time in HH:MM format, e.g.: 08:30, 16:00
* UNIT: Name of the lesson's unit, e.g.: ITSFT-406-1502 - Programming Concepts

An example of a week configuration is found below:
```csv
Mon,IT-SWD-6.2A,08:00,10:00,ITSFT-506-1614 - Low Level Programming II
Mon,IT-SWD-6.2B,10:00,12:00,ITSFT-506-1614 - Low Level Programming II
Mon,IT-MSD-4.2B,12:30,14:00,ITSFT-406-1502 - Programming Concepts
Tue,IT-MSD-4.2C,10:30,12:00,ITSFT-406-1502 - Programming Concepts
Wed,IT-MSD-4.2B,08:30,10:00,ITSFT-406-1502 - Programming Concepts
Wed,IT-SWD-6.2A,10:00,12:30,ITSFT-506-1614 - Low Level Programming II
Thu,IT-SWD-6.2A,08:00,10:30,ITSFT-506-1614 - Low Level Programming II
Thu,IT-MSD-4.2C,12:30,14:00,ITSFT-406-1502 - Programming Concepts
Fri,IT-MSD-4.2B,08:00,09:30,ITSFT-406-1502 - Programming Concepts
Fri,IT-MSD-4.2C,10:30,12:00,ITSFT-406-1502 - Programming Concepts
```
