
# EX.NO : 3(A)  INHERITANCE(BASE CLASS & DERIVED CLASSES) 

# PROGRAM STATEMENT :  
write a c++ program to read 3 employee details(empno,empname & empgender) in one class and display 
their details in another class using inheritance? 

# ALGORITHM:    
1. Start the program.  
2. Define a class A with protected attributes regno, name, and gender, and a public method get to read values for these attributes.  
3. Define a derived class B that inherits from class A and includes a display method to output the employee details.  
4. In the main function, create an object obj of class B, call get to read input, and then call display to print the employee details.  
5. End the program.

# PROGRAM:
```
#include <iostream>
using namespace std;

class A {
public:
    int empno;
    string empname, empgender;

    void getDetails() {
        cin >> empno >> empname >> empgender;
    }
};

class B : public A {
public:
    void displayDetails() {
        cout << empno << " " << empname << " " << empgender << endl;
    }
};

int main() {
    B employees[3];
    
    for (int i = 0; i < 3; i++) {
        employees[i].getDetails();
    }
    cout << "Employee Detaile are" << endl;
    for (int i = 0; i < 3; i++) {
        employees[i].displayDetails();
    }
    return 0;
}
```
# output:

![Screenshot 2025-05-27 103148](https://github.com/user-attachments/assets/5f93037c-1a5d-40cd-9957-a65b044dd8c1)

# Result:  
Thus, the C++ program to read empno,empname & empgender in one class and display the above details in another class using inheritance is created successfully. 
