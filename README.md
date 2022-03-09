

Question 1 of 27 Next Question Last QuestionUnsaved change Moving to another question will save this response.
Question 1

Using MPI, write a parallel linear search program that searches for a given key in an array of n integers. Do “copy and paste” of the following serial code to fill your answer area. Declare, initialize, and use any variables or objects you need for your program. Include essential lines of code needed to complete the main() function and modify the search function with correct parameters and appropriate code-lines for handling a thread. No credit will be given if you don't use the given code for your solution. The solution must be valid for any integer n.

#include <stdio.h>

int linearSearch(int arr[], int n, int key)

{

    int i;

    for (i = 0; i < n; i++)

        if (arr[i] == key)

            return i;

    return -1;

}

int main(void)

{

    int arr[] = { 2, 3, 4, 10, 40, 50, 60, 70, 80, 90 }; // Example elements

    int key;

    scanf(“%d”,&key);

    int n = sizeof(arr) / sizeof(arr[0]);

    int result = linearSearch(arr, n, key);

   (result == -1)? printf("Element is not present in array\n");

                 : printf("Element is present at index %d\n",result);

   return 0;

}
