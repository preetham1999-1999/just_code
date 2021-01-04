#include <iostream>
#include<stack>
using namespace std;

int main()
{
   string s1 = "Hello";
   string s2 = "World";
   stack<char> ss;
   
   for(int i=s2.length(); i>=0; i--){
       ss.push(s2[i]);
   }
   ss.push(' ');
   for(int i=s1.length(); i>=0; i--){
       ss.push(s1[i]);
   }
    while (!ss.empty()) { 
        cout <<ss.top(); 
        ss.pop(); 
    }
}
