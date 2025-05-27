
# EX.NO : 3(B)  PROTECTED MEMBERS & OVERRIDING 

# PROGRAM STATEMENT :  
To write a c++ program to implement protected member with character values.  

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
class Base {
protected:
    char n; 
};
class Derived : public Base {
public:
    void func() {
        cin >> n;
        cout << "The value of n is: " << n << endl;
    }
};
int main() {
    Derived obj;
    obj.func();  
    return 0;
}
```
# output:

![Screenshot 2025-05-27 103922](https://github.com/user-attachments/assets/78d617b5-6977-4df4-89fa-cfc19e1e6465)

# Result:

Thus, the C++ program to implement protected member with character values is created successfully.  
