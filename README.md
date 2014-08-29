CS211_Project
=============

Final Project from Programming for Engineers I in C

Project
=======

Write a C program which can read a list of strings from the user and print them to the screen. This list must be stored as a doubly-linked list (with a tail pointer) of pointers to the actual string data. There must be no limit placed on the length of the individual strings in this list, and the strings themselves must be allocated dynamically, to the exact size required to store the full string, including the null. These strings may be read in the same way as in lab #4, each being a whole line, terminated by a null. You should re-use that code in this lab.

You must provide the ability to both save and load this entire list to and from a text file. The format of this file should simply be one string per line, until the end of the file.

You must create a function which will swap the location of two strings between two nodes. You should do this by swapping the pointers to the strings, not by rearranging the nodes themselves.

For this list of strings, you should implement each of the following sorting algorithms to sort them in alphabetical order (the order created by comparing with the C strcasecmp() function is fine):

1. Selection Sort
2. Insertion Sort
3. Bubble Sort (Bi-Directional)
4. Quick Sort (Pick First For Pivot)
5. Quick Sort (Pick Middle For Pivot)

Each sort should count how many swaps are required to put the list of strings in order, using the swap function require above.

Your first main program should be a basic interactive program to manipulate the list (including at least the ability to insert values at the end or beginning, remove the last or first element, add a list of strings, remove a particular string, search for a particular string, etc...).

You should write a second main program which non-interactively loads a text file of strings whose name was specified on the command line as the only argument to the program. This list should be sorted by each of the required algorithms, and the number of swaps required should be printed for each.

Your Makefile must be written such that running "make" will build both of these programs. Both must use the same code for working with the list itself, by including the same header files and linking in the same object files in the Makefile. Only the code for the main function should be different between them.
