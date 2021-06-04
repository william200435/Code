# Code
```
#include<iostream>
using namespace std;

int stack[105], stack_top;

int main (){
    string cmd;
    int i;
    stack_top = 0;
    while( cin >> cmd )    {
        if( cmd == "push" )
        {
            cin >> i;
            stack[stack_top] = i;
            stack_top++;
        }
        else if( cmd == "pop" )
        {
            if( stack_top == 0 )
                cout << " pop: nothing in stack" << endl;
            else
            {
                cout << " pop: " << stack[stack_top-1] << endl;
                stack_top--;
            }
        }
    }
    return 0;
}
```
