# C++


#include<iostream>
using namespace std;
int main()
{
  cout<<"We will see what is syntax of C++ Lnguage.\n";
  /*
  #include <iostream>
  using namespace std;
  int main()
  {
     CODE
     return 0;
  }
  */
  cout<<"We gonna learn C++ Language from now on. \n";
  cout<<"We'll see how to set constant values of any variable by using \'const\' keyword. \n";
  
  const int Deep = 21;
  cout << Deep <<"\n";
  
  cout<< "Now we will see how we can take user input by using \'cin >>\' \n Let's first declare any variable and ask the user to put the value to it. \n";
  
  string Name;
  int Age;
  cout << "Please Enter your Name - ";
  cin >> Name;
  cout <<"Please Enter your age - ";
  cin >> Age;
  
  cout<<"Now we'll learn about the Operators in C++: \n 1) Arithmetic Operators \n 2) Assignment Operators \n 3) Comparison Operators \n 4) Logical Operators \n 5) Bitwise Operators \n\n";
  cout<<"Arithmetic Operators include - \'+\', \'-\', \'*\', \'/\', \'%\', \'++\', \'--\'. \n\n";
  cout<<"Assignment Operators include - \'+=\', \'-=\', \'*=\', \'/=\', \'%=\'.\n\n";
  cout<<"Comparison Operators include - \'=\', \'!=\', \'>\', \'<\', \'>=\', \'<=\'. \n\n";
  cout<<"Logical Operators include - \'&&\', \'||\', \'!\'. \n\n";
  
    cout<<"Let's talk about the Strings.\n If we ever need to use strings, we need to include \"#include<string>\" library.\n";
    cout<<"We can use strings by \'string variableName = \"Value\" \' this format, and the value we are assigning to the variable will be in double quotes.\n";
    cout<<"We can concatenate the strings by using \'+\' operator or by using \'string1.append(string2);\', but here is awarning that C++ uses \'+\' operator for concatenation and addition, like if we add two numbers the result will be a number, if we add two strings the result will be a string.";
    
    
    
  
  return 0;
}
