# CIS278-Programming-Project-3-solution

Download Here: [CIS278 Programming Project #3 solution](https://jarviscodinghub.com/assignment/cis278-programming-project-3-solution/)

For Custom/Original Work email jarviscodinghub@gmail.com/whatsapp +1(541)423-7793

For this project, you are to implement a simple class registration list, with associated wait list. Your program will use two arrays, one to store ID numbers of students who are registered in the class, and one to store ID numbers of students who are waitlisted. Both of these arrays will be partially filled arrays (see text pages 196).

The Application

The application is to maintain two arrays, one for registered and one for waitlisted students. Each array stores the int id number of the students. Your arrays should be declared within the main function (not globally outside all functions), and passed as arguments to any function that needs them. As indicated in the text, in addition to having a variable to store the capacity of the array, you will also need a variable to keep track of how many values are currently stored in each array.

The application should allow the user to do one of 5 things, until he/she wishes to exit:
* register a student
* unregister a student
* print list of registered students
* print wait list

Make sure of that if a student wishes to be registered, but the class is full, the student is added to the waitlist, unless that list is also full. You can use both class lists and waitlists of size 10 for this assignment, use a constant variable for the size.

When a student is unregistered, if the waitlist is not empty, the next student on the waitlist should be moved from the waitlist to the class list.

The main program is to call the function ‘getId’ (see below) each time an id is needed from the user. You may want to get your program running correctly with usual int input prior to introducing this function (or test and debug the function getId in a separate main program).

Your program is to accomplish each of the following by calling upon the following functions (which you must provide):

Precondition: array is not full (ie however, array may not yet any contain values)
Postcondition: array contains one more value, it follows all preexisting values
void addToRear(int arr[], int& howmany, int value)
This function adds one new element, value, to the array. The parameter ‘howmany’ is the
number of values currently stored in the array.

Precondition: array is not empty
Postcondition: array contains one less value,
int removeFromFront(int arr[], int & howmany)
This function removes a value from the front of the array, and shuffles remaining elements up .
Value which was removed is returned by this function. The parameter ‘howmany’ is updated to
reflect the number of values currently stored in the array.

Precondition: ‘value’ exists in the array
Postcondition: array contains one less value,
int remove(int arr[], int& howmany, int value)
This function removes ‘ value’ from the array, and readjusts other elements
Value which was removed is returned by this function.

Precondition: none
Postcondition: array is not changed
void printArray(int arr[], int howmany)
This function outputs the elements which are stored in the array.

Precondition: none
Postcondition: arr is not changed
bool isFull( int capacity, int howmany)
This function determines if the array is full.

Precondition: none
Postcondition: arr is not changed
bool isEmpty( int howmany)
This function determines if the array is empty.

Precondition: none
Postcondition: value contains valid id number
void getId( int& value)
This function inputs in a Cstring, removes all non digit characters, and converts the remaining
chars into an int value. (Recall, a Cstring is a null terminated char array).

eg input 11a1
value 111

____________________________________________________________

Submit in your program, in a file named ‘register.cpp’ , as an email attachment. Tradtional class students please hand in a hard copy.
