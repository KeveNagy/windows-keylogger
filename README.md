# Keve's notes for this fork
I found Faraj Farook's code to be a very promising and very educational proof-of-concept solution to a **keyboard and mouse input logging** challenge I have been interested in. His source helped me to confirm that what I had on mind is actually doable, and it saved me a considerable amount of time and effort by showing **HOW** it can be done. So I am grateful, and much appreciate that he shared his work publicly.
The original [farajfarook/windows-keylogger](https://github.com/farajfarook/windows-keylogger) code is very spartaic though. And I have plans to extend it with many essential convenience and usability functions it lacks, plus customise it to my specific needs for academic research purposes in an educational environment. Hence this fork was made.

For now, I leave the original contents of the README below.

---

# Windows Keylogger
User Mode - Windows Key Logger application for educational purposes

This application will capture all your keyboard key press events and save it in a file in the background.!

**disclaimer** *This application is created with no warranty or neither I would take any responsibilities for any sort of threats imposed by any individual or a group of individuals towards anyone. This application is developed soley for educational purposes of learning how Windows C++ API works in global keyboard hooks*

## Getting started
#### Steps to build
1. Clone the repository to your local PC
2. Open the solution with visual studio with C++
3. Build the project

#### Steps to execute/kill

1. Get the executables from the build folder, and execute the `keylogger.exe`
2. To kill the process you have to open up the `task manager` and search the process and kill it.

## More information
Application is designed to write a file with the name `keylogger.txt` which contains all the key press done in the windows host where this application is running. This file is created along with the `exe` file which is excuted. You can change this file name from the `stdafx.h` file's line: `#define LOGFILE "keylogger.txt"`

In the debug mode application is written to write back to the log output window. 

Application is **Unicode enabled.** So if the keyboard input has some extraordinary characters those will also get logged in the file.

  - Update me with the bug as posting new issues in the github.
  - Feel free to fork the project and fix any bugs that you find.
  - have fun!
