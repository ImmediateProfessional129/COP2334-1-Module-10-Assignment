# COP2334-1-Module-10-Assignment
This is a repository link of the COP2334-1 Module 10 Assignment

// This program is designed to tally the amount of characters such as letters that are in a string like a word or sentence written by the user.

// Include the library statements.
#include <iostream>
#include <string>
using namespace std; // Using standard namespace.

int StringAmount(char *str); // Function tool for the StringAmount operator to add the amount of characters in a string.

int main() { // Main function.
  const int LENGTH = 80; // Constant integer for the length of the string.
  char str[LENGTH]; // Character array for the string.
  cout << "Enter a string like a word or a full sentence: "; // Prompt the user to enter a string.
  cin.getline(str, LENGTH); // Get the string from the user.
  cout << "The string has " << StringAmount(str) << " characters." << endl; // Display the amount of characters in the string.
  return 0; // Return 0 for the main function to execute the program.
}

int StringAmount(char *str) { // Function tool for the StringAmount operator to add the amount of characters in a string.
  int count = 0; // Integer for the count of the characters in the string.
  while (*str != '\0') { // While loop to add the amount of characters in the string.
    count++; // Add an additional 1 to the count of the characters in the string.
    str++; // Add an additional 1 to the string also.
  }
  return count; // Return the count of the characters in the string.
}
