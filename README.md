# Experiment-9

Aim:
To study and implement C++ Pointer basics

Theory:
Pointers in C++ denote variables that hold the address of another variable in memory. They permit direct memory operation thus playing an essential role in specific programming tasks like dynamic storage allocation, matrices, and also developing complex data structures e.g. linked list and trees. A pointer gets declared when a data type is defined with the sign ‘*’ before writing down the name of the pointer itself after it. This indicates what kind of variable does this point towards. The & operator used delivers a variable’s physical location in a computer’s storage space. This operator can retrieve or reference what is held by an address number which is stored within its range. This means that dereferencing enables one to read as well as alter certain values belonging to that particular place you arrived at pointing still added onto them. Pointers can get lengthened or shortened so as they lead to areas right above ours or below depending on whatever you want them to do with your pointers; particularly amid arrangements involving arrays where these may become more useful by calling upon different addresses thereby traversing through all their parts simultaneously.

Code:
```
#include <iostream>
using namespace std;
int main()
{
    int a,b;
    int *i, *j;
    int k;
    cout<<"Enter a number: ";
    cin>>a;
    cout<<"Enter another number: ";
    cin>>b;
    i = &a;
    j = &b;
    cout<<"Memory location of first number : "<<i<<endl;
    cout<<"Memory location of first number : "<<&a<<endl;
    cout<<"First number using dereferencing : "<<*i<<endl;
    cout<<"First number : "<<a<<endl;
    cout<<"Memory location of first number : "<<j<<endl;
    cout<<"Memory location of first number : "<<&b<<endl;
    cout<<"Second number : "<<*j<<endl;
    cout<<"Second number : "<<b<<endl;
    cout<<"Sum of two numbers: "<<*i+*j<<endl;

    for (k = 0;k<3;k++)
    {
        i++;
        cout<<"Incremented memory: "<<i<<endl;
    }
    *i = 20;
    cout<<a<<endl;

    int c[] = {1,2,3,4,5};

    cout<<"Array as a pointer: "<<*c<<endl;

    cout<<"Array pointer with iteration: "<<endl;
    for (k = 0; k<5 ;k++)
    {
        cout<<*(c+k)<<endl;
    }
}
    ```
OUTPUT:-
![Ex 9 JPG](https://github.com/user-attachments/assets/e0d0f874-7fc0-48ad-933f-7901bd028699)


Conclusion- We learned how to use pointers in C++.
