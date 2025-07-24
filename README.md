#include <iostream>
using namespace std;

int main() {
    double num1, num2, result;
    int choice;

    do {
        // Display menu
        cout << "\n==== Simple Calculator ====" << endl;
        cout << "1. Addition (+)" << endl;
        cout << "2. Subtraction (-)" << endl;
        cout << "3. Multiplication (*)" << endl;
        cout << "4. Division (/)" << endl;
        cout << "5. Exit" << endl;
        cout << "Choose an operation (1-5): ";
        cin >> choice;

        // Exit if user chooses 5
        if (choice == 5) {
            cout << "Thank you for using the calculator!" << endl;
            break;
        }

        // Input numbers
        cout << "Enter first number: ";
        cin >> num1;
        cout << "Enter second number: ";
        cin >> num2;

        // Perform selected operation
        switch (choice) {
            case 1:
                result = num1 + num2;
                cout << "Result: " << result << endl;
                break;
            case 2:
                result = num1 - num2;
                cout << "Result: " << result << endl;
                break;
            case 3:
                result = num1 * num2;
                cout << "Result: " << result << endl;
                break;
            case 4:
                if (num2 != 0) {
                    result = num1 / num2;
                    cout << "Result: " << result << endl;
                } else {
                    cout << "Error: Division by zero is not allowed!" << endl;
                }
                break;
            default:
                cout << "Invalid choice! Please select between 1 and 5." << endl;
        }

    } while (true);

    return 0;
}
# c-program-proj-2
