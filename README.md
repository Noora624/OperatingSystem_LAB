Lab Experiment Sheet-1
OS Lab Assignment 1 - Process Creation and Management
📘 Course Info

Course Code & Name: ENCS351 - Operating System
Program: B.Tech CSE, AI/ML, Data Science, Cyber, FSD, UX/UI
Experiment Title: Process Creation and Management Using Python OS Module
Date & Time: Created on Tuesday, September 16, 2025, 11:17 PM IST


🎯 What’s This About?
This lab is all about messing around with Linux processes using Python! You’ll:

Mimic fork(), exec(), and check process states.
Play with zombie and orphan processes (spooky, right?).
Peek into /proc to see process details.
Test priority scheduling with nice() values.


📝 What to Do

Process Creation Utility
Make N child processes with os.fork(). Each kid shows its PID, parent PID, and a "Hello" message. The parent waits for everyone to finish.
Command Execution Using exec()
Turn Task 1 into a command runner! Each child runs a Linux command like ls or date.
Zombie & Orphan Processes

Zombie: Fork a kid and let the parent skip wait()—check with ps -el | grep defunct.
Orphan: Parent bails before the child finishes.


Inspecting Process Info from /proc
Type a PID, then dig into /proc/[pid]/status for name, state, memory, /proc/[pid]/exe for the executable, and /proc/[pid]/fd for open files.
Process Prioritization
Spin up CPU-hogging kids with different nice() values and see who finishes first!


📂 Files You’ll Need

task1.py → Code for Task 1 (Process Creation)
task2.py → Code for Task 2 (Command Execution)
task3.py → Code for Task 3 (Zombie & Orphan)
task4.py → Code for Task 4 (Process Inspection)
task5.py → Code for Task 5 (Prioritization)
output.txt → Log of what happens when you run these
report.pdf → Your report with goals, code, and results
README.md → This guide (you’re here!)


🚀 How to Use This

Get Ready: Use a Linux machine with Python 3 installed.
Run Each Task:

Open a terminal, go to the folder with these files.
Run a task with python3 task1.py > output.txt (or task2.py, task3.py, etc.).
Check output.txt for the results!


Tips:

Task 1: Pick a number (e.g., 3) when asked.
Task 2: Type a command like ls or date.
Task 3: Pick 1 for zombie or 2 for orphan; open another terminal for ps -el | grep defunct.
Task 4: Enter a PID (try your own with ps).
Task 5: Let it run 5 seconds to see the priority effect.


Save Output: Redirect to output.txt as shown above for your report.


🤓 Extra Notes

Stick to Linux—/proc stuff won’t work on Windows.
If a command fails (e.g., Task 2), double-check your spelling.
Have fun debugging! If stuck, ask me or your lab buddy.

Happy coding! 😄