# Student-Management-System
Student management system using C++

Student Record Management System
Overview
The Student Record Management System is a console-based application developed in C++ designed to manage student records efficiently. This project allows users to enter, display, search, update, and delete student data. It provides a simple yet effective way to manage student information using arrays and basic input/output operations.

Features
Enter Data: Allows users to input and store information for multiple students. Each student record includes Roll Number, Name, Class, Course, Mobile Number, and Admission Year.
Show Data: Displays the stored information for all students.
Search Data: Enables users to search for a specific student's data using their Roll Number.
Update Data: Allows users to update the details of a specific student by providing their Roll Number.
Delete Data: Gives an option to delete all student records from the system.
Code Explanation
Data Storage
The application uses arrays to store student information:

cpp
Copy code
string roll_no[30], name[30], Class[30], course[30], mobile_no[30], admission_year[30];
int total = 0;
These arrays hold the Roll Number, Name, Class, Course, Mobile Number, and Admission Year for up to 30 students.

Functions
Enter Data: enter() function collects and stores student information.
Show Data: show() function displays the information of all students.
Search Data: search() function allows searching for a student by Roll Number.
Update Data: update() function updates the details of a specific student.
Delete Data: Delete() function deletes all student records from the system.
Main Function
The main() function provides a menu-driven interface for the user:


int main() {
    int value;
    while (true) {
        cout << "\nPress 1 to Enter data" << endl;
        cout << "Press 2 to Show data" << endl;
        cout << "Press 3 to Search data" << endl;
        cout << "Press 4 to Update data" << endl;
        cout << "Press 5 to Delete data" << endl;
        cout << "Press 6 to Quit" << endl;
        cin >> value;

        switch (value) {
            case 1: enter(); break;
            case 2: show(); break;
            case 3: search(); break;
            case 4: update(); break;
            case 5: Delete(); break;
            case 6: exit(0); break;
            default: cout << "Invalid input" << endl; break;
        }
    }
}
The menu allows users to choose different operations like entering, displaying, searching, updating, and deleting student records.

Usage
Entering Data: The user is prompted to enter the number of students and then input details for each student.
Displaying Data: Displays all student records.
Searching Data: Prompts the user to enter a Roll Number and displays the corresponding student's details.
Updating Data: Allows updating the details of a specific student by Roll Number.
Deleting Data: Deletes all student records after confirmation.
Quit: Exits the application.
