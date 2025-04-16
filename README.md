// Create An Array Operation
// Push operation to add an element in Stack 

#include <iostream>                 //  headers — input/output ke liye
using namespace std;

#define SIZE 5                  // Stack ka size 5 define kiya
int myStack[SIZE];             //   myStack[] naam ka array banaya to store values
int top = -1;                  //  top = -1 means stack is initially empty

void push(int value){
    if (top == SIZE )
    {
        cout<< " Stack Overflow\n";
    }else{
        top++;
        myStack[top] = value;
        cout<<value << " push into Stack\n";
    }
}
// stack me push operation tab tak hota hai jab tak stack full na ho jaaye.
// Stack overflow check karne ke liye top == SIZE - 1 use karte hain.
// Har push ke baad top increase hota hai aur value stack me store hoti hai
 int main(){
     push(10);
     push(20);
     push(30);
    
     return 0;
 }
