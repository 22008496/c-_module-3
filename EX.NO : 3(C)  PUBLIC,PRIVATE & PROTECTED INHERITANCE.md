
# EX.NO : 3(C)  PUBLIC,PRIVATE & PROTECTED INHERITANCE  
# PROGRAM STATEMENT :  
Write a C++ program to get two numbers from two base classes and display the product of two numbers in the derived class. 

# ALGORITHM:    
1. Start the program.  
2. Define a class Snake with integer attributes a, b, c, and d, and a method get to read values for these attributes.  
3. Define a class Cobra that inherits from Snake and includes a method pro to calculate and display the product of a and b.  
4. In the main function, create an object obj of class King, call get to read input values, call pro to display the product of a and b.  
5. End the program.

# PROGRAM:
```
#include <iostream>
using namespace std;
class A {
protected:
    int num1;
public:
    void setNum1(int n) {
        num1 = n;
    }
};
class B {
protected:
    int num2;
public:
    void setNum2(int n) {
        num2 = n;
    }
};
class C : public A, public B {
public:
    void displayProduct() {
        cout << "Product of two numbers = " << num1 * num2 << endl;
    }
};

int main() {
    C obj;
    int a, b;
    cin >> a >> b;
    obj.setNum1(a);
    obj.setNum2(b);
    obj.displayProduct();

    return 0;
}
```

# output:

![Screenshot 2025-05-27 104526](https://github.com/user-attachments/assets/6e8866c8-440f-4d8b-bf61-5e9b1851e4af)

# Result:

Thus, the C++ program to find product of two numbers using Hierarchical inheritance is created successfully. 
