# Calculator-using-C-
Beginner-friendly calculator 
#include <iostream>

using namespace std;

int main() {

double num1, num2, result; // Variables for numbers and result

char operation; // Variable for operation choice

// Welcome message

cout << "Welcome to the Beginner's Calculator!" << endl;

cout << "This program can add (+), subtract (-), multiply (*), or divide (/)." << endl;

// Get user input

cout << "Enter your first number: ";

cin >> num1;

cout << "Choose an operation (+, -, *, /): ";

cin >> operation;

cout << "Enter your second number: ";

cin >> num2;

// Perform the chosen operation

if (operation == '+') {

result = num1 + num2;

cout << num1 << " + " << num2 << " = " << result << endl;

}

else if (operation == '-') {

result = num1 - num2;

cout << num1 << " - " << num2 << " = " << result << endl;

}

else if (operation == '*') {

result = num1 * num2;

cout << num1 << " * " << num2 << " = " << result << endl;

}

else if (operation == '/') {

if (num2 != 0) { // Check for division by zero

result = num1 / num2;

cout << num1 << " / " << num2 << " = " << result << endl;

}

else {

cout << "Error: Cannot divide by zero!" << endl;

}

}

else {

cout << "Error: Invalid operation! Please use +, -, *, or /" << endl;

}

cout << "Thank you for using the calculator!" << endl;

return 0;

}
