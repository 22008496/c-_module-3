
# EX.NO : 3(D)  CONSTRUCTOR & DESTRUCTOR IN DERIVED CLASS 
# PROGRAM STATEMENT :  
Write a C++ program to pass a character to the parameterized constructor of the base class through derived class constructor. 
# ALGORITHM:    
1. Start the program.  
2. Define a class Parent with a public string attribute n initialized to "j", and a constructor that outputs the password passed to the base class.  
3. Define a class Child that inherits from Parent and has a constructor that outputs the password received from the base class.  
4. In the main function, create an object c of class Child, which automatically calls the constructors of both Parent and Child to display the messages.  
5. End the program.
   
# Program: 
```
#include <iostream>
using namespace std;
class Parent {
public:
    Parent(char c) {
        cout << " The value passed to the base class is " << c << endl;
    }
};
class Child : public Parent {
public:
    Child(char c) : Parent(c) {
        cout << "The value " << c << " is passed through the derived class constructor" << endl;
    }
};
int main() {
    char inputChar;
    cin >> inputChar;
    Child obj(inputChar);
    return 0;
}
```
# output:

![Screenshot 2025-05-27 105006](https://github.com/user-attachments/assets/c31cc946-6388-45d3-a821-e1785c4cb3b4)

# Result: 
Thus, the C++ program to pass a password (j )to the parameterized constructor of a base class through the derived class constructor is created successfully. 
