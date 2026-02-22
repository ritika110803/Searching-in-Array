 C Program: Linear Search in an Array

This project demonstrates how to implement the *Linear Search* algorithm in the C programming language.

 Description

The program:

* Declares and initializes an integer array
* Accepts a number from the user
* Searches for the number using a *linear search algorithm*
* Displays the position of the element if found
* Displays a message if the element is not found

This is a beginner-friendly example for understanding searching techniques in C.

---

 Source Code

c
#include <stdio.h>

int main() {
    int arr[] = {10, 25, 30, 45, 50};
    int n = 5;
    int key, i;
    int found = 0;

    printf("Enter number to search: ");
    scanf("%d", &key);

    for(i = 0; i < n; i++) {
        if(arr[i] == key) {
            printf("Element found at position %d\n", i + 1);
            found = 1;
            break;
        }
    }

    if(found == 0) {
        printf("Element not found\n");
    }

    return 0;
}


---

 How to Compile and Run

 Using GCC

1. Save the file as linear_search.c
2. Open terminal or command prompt
3. Compile the program:


gcc linear_search.c -o linear_search


4. Run the executable:


./linear_search


(On Windows, use linear_search.exe)

---

 Sample Output

 ✅ When Element is Found


Enter number to search: 30
Element found at position 3


 ❌ When Element is Not Found


Enter number to search: 100
Element not found


---

 Concepts Covered

* Arrays in C
* User input using scanf()
* Looping with for
* Conditional statements (if)
* Linear Search Algorithm

---

 Algorithm Steps

1. Start
2. Initialize array
3. Take input from user
4. Compare input with each array element
5. If match found → display position
6. If no match found → display "Element not found"
7. End

---
