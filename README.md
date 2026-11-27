Student Name: J K ANJANAI

Register Number: 1911260255

Subject: C Programming

Assignment Number: 5

Topic: Storage Classes – The Same Counter Four Ways

1. Compiler and Version

Compiler: GCC (GNU Compiler Collection)

Version: Check the installed GCC version using:

gcc --version

Record the version displayed by your system.

2. Programs and Compilation Commands

Task 5.1 – Four Implementations

1. Automatic Local Variable

File: task5_automatic.c

Compilation:

gcc task5_automatic.c -o automatic

Execution:

./automatic

Result: Displays 1001 for every function call because the automatic variable is initialized again each time.

2. Static Local Variable

File: task5_static.c

Compilation:

gcc task5_static.c -o static

Execution:

./static

Result: Generates consecutive token numbers 1001, 1002 and 1003 because the static variable retains its value between function calls.

3. Global Variable Using extern

Files: main.c and token.c

Compilation:

gcc main.c token.c -o global

Execution:

./global

Result: Generates consecutive token numbers 1001, 1002 and 1003 using a global variable shared between two source files.

4. Register Variable

File: task5_register.c

Compilation:

gcc task5_register.c -o register

Execution:

./register

Result: Displays token numbers from 1001 to 1003 using a register variable in a loop.

Task 5.1 – Complete the Code (TODO 1)

File: task5_completed_program.c

Compilation:

gcc task5_completed_program.c -o completed

Execution:

./completed

Result: Demonstrates the difference between static and automatic variables. Static generates 1001, 1002 and 1003, while automatic generates 1001 repeatedly.

Task 5.2 – Two Independent Counters

1. Pointer-Based Counters

File: task5_two_counters.c

Compilation:

gcc task5_two_counters.c -o counters

Execution:

./counters

Result: Generates two independent sequences for vegetarian and non-vegetarian tokens, both starting from 1001.

2. Static Independent Counters

File: task5_static_two_counters.c

Compilation:

gcc task5_static_two_counters.c -o static_counters

Execution:

./static_counters

Result: Uses two separate static variables to maintain independent vegetarian and non-vegetarian token sequences.

3. Global Independent Counters

Files: main.c and token.c (two-counter implementation)

Compilation:

gcc main.c token.c -o global_counters

Execution:

./global_counters

Result: Uses two global counters shared between source files through the extern keyword.

4. Register-Based Counters

File: task5_register_two_counters.c

Compilation:

gcc task5_register_two_counters.c -o register_counters

Execution:

./register_counters

Result: Displays separate vegetarian and non-vegetarian token sequences using register loop variables.

3. General Program Execution Instructions

Open the Assignment 5 folder in VS Code or a terminal.

Make sure GCC is installed.

Open the terminal in the project directory.

Use the corresponding GCC compilation command.

Run the generated executable.

Check the output against the expected result.

Upload the source files and this README.md file to GitHub.

Note: On Windows, use the generated .exe file to execute the programs, for example automatic.exe.

4. Conclusion

This assignment demonstrates the four storage classes in C: automatic, static, global and register. It explains their scope, lifetime, initialization and value retention. It also demonstrates how independent counters can be maintained using static variables, global variables and pointers.
