#include <iostream.h>
#include <conio.h>
// Function to add two numbers
int add(int a, int b) {
    return a + b;
}
// Function to subtract two numbers
int subtract(int a, int b) {
    return a - b;
}
// Function to multiply two numbers
int multiply(int a, int b) {
    return a * b;
}
// Function to divide two numbers
double divide(int a, int b) {
    if (b == 0) {
        cout << "Error: Division by zero!" << endl;
        return 0;
    }
    return (double)a / b;
}

// Function to calculate the area of a rectangle
int rectangleArea(int length, int width) {
    return length * width;
}

// Function to calculate the area of a circle
double circleArea(int radius) {
    return 3.14159 * radius * radius;
}
void  main() {
    int choice, num1, num2, length, width, radius;
    cout << "Simple Calculator Program" << endl;
    cout << "1. Addition" << endl;
    cout << "2. Subtraction" << endl;
    cout << "3. Multiplication" << endl;
    cout << "4. Division" << endl;
    cout << "5. Rectangle Area" << endl;
    cout << "6. Circle Area" << endl;
    cout << "Enter your choice (1-6): ";
    cin >> choice;

    switch (choice) {
        case 1:
            cout << "Enter two numbers: ";
            cin >> num1 >> num2;
            cout << "Result: " << add(num1, num2) << endl;
            break;
        case 2:
            cout << "Enter two numbers: ";
            cin >> num1 >> num2;
            cout << "Result: " << subtract(num1, num2) << endl;
            break;
        case 3:
            cout << "Enter two numbers: ";
            cin >> num1 >> num2;
            cout << "Result: " << multiply(num1, num2) << endl;
            break;
        case 4:
            cout << "Enter two numbers: ";
            cin >> num1 >> num2;
            cout << "Result: " << divide(num1, num2) << endl;
            break;
        case 5:
            cout << "Enter length and width of rectangle: ";
            cin >> length >> width;
            cout << "Area: " << rectangleArea(length, width) << endl;
            break;
        case 6:
            cout << "Enter radius of circle: ";
            cin >> radius;
            cout << "Area: " << circleArea(radius) << endl;
            break;
        default:q
            cout << "Invalid choice!" << endl;
            break;
            getch();
    }
