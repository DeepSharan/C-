# C++


#include<iostream>
#include<string>
#include<cmath>  
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
  int Age, x, y, Add, Sub, Multiply, Mod, Divide;
  cout << "Please Enter your Name - ";
  cin >> Name;
  cout <<"Please Enter your age - ";
  cin >> Age;
  
  cout<<"Now we'll learn about the Operators in C++: \n 1) Arithmetic Operators \n 2) Assignment Operators \n 3) Comparison Operators \n 4) Logical Operators \n 5) Bitwise Operators \n\n";
  cout<<"Arithmetic Operators include - \'+\', \'-\', \'*\', \'/\', \'%\', \'++\', \'--\'. \n";
  cout<<"Input two numbers: ";
  cin >> x >> y;
  Add = x+y;
  Sub = x-y;
  Multiply = x*y;
  Divide = x/y;
  Mod = x%y;
  cout<<"Addition (x + y) = "<<Add <<"\n";
  cout<<"Subtraction (x - y) = "<<Sub <<"\n";
  cout<<"Multiplication (x * y) = "<<Multiply <<"\n";
  cout<<"Divide (x / y) = "<<Divide <<"\n";
  cout<<"Modulus (x % y) = "<<Mod <<"\n";
  cout<<"Increment (++x) = "<<++x <<"\n";
  cout<<"Decrement (--x) = "<<--y <<"\n\n";
  
  cout<<"Assignment Operators include - \'+=\', \'-=\', \'*=\', \'/=\', \'%=\'.\n\n";
  cout<<"Comparison Operators include - \'=\', \'!=\', \'>\', \'<\', \'>=\', \'<=\'. \n\n";
  cout<<"Logical Operators include - \'&&\', \'||\', \'!\'. \n\n";
  
    cout<<"Let's talk about the Strings.\n If we ever need to use strings, we need to include \"#include<string>\" library.\n";
    cout<<"We can use strings by \'string variableName = \"Value\" \' this format, and the value we are assigning to the variable will be in double quotes.\n";
    cout<<"We can concatenate the strings by using \'+\' operator or by using \'string1.append(string2);\', but here is a warning that C++ uses \'+\' operator for concatenation and addition, like if we add two numbers the result will be a number, if we add two strings the result will be a string.";
    cout<<"We can access and change the elements of the strings by using \"stringname[] = \' \' ;\" this. \n";
    cout<<" The C++ language only takes one word as input from the user, cuz \'cin\' considers a whitespace, and takes the space as terminating character, so to input a line we use \"getline(cin, stringName)\". Let\'s take a example further.\n";
    string Ans;
    cout<<"Hey! What\'s your Full Name ? \n";
    getline(cin, Ans);
    cout<<"So, you are "<<Ans <<"\n\n";
    
    cout<<"We can perform mathematical tasks on numbers by using \' include<cmath> \' header file. \n This will include functions like \' sqrt(squareroot) \', \' round(rounds a number) \', \' log(natural logarithm) \', and many other functions. \n We can also find the maximum value between any numbers using \' max( ) \' function and the minimum value using \' min ( ) \' function.\n";
    int a;
    cout << "Input a number = ";
    cin >> a;
    cout<<"Square root of "<< a <<" is "<< sqrt(a) <<"\n";
    cout<<"Round off of "<< a <<" is "<< round(a) <<"\n";
    cout<<"Log of "<< a <<" is "<< log(a) <<"\n\n";
    
    cout<<"Let\'s jump to the switch statements. \n In this, there are many cases given but we need to specify that which code we want to execute.\n Let\'s see an example by taking an input from the user.\n";
    int day;
    cout<<"Enter a day number: ";
    cin >> day;
    switch(day)
    {
      case 1:
      cout<<"Monday";
      break;
      case 2:
      cout<<"Tuesday";
      break;
      case 3:
      cout<<"Wednesday";
      break; 
      case 4:
      cout<<"Thursday";
      break;
      case 5:
      cout<<"Friday";
      break;
      case 6:
      cout<<"Saturday";
      break;
      case 7:
      cout<<"Sunday";
      break;
      default:
      cout<<"You are a fool :)";
    }
    
    cout<<"Now we\'ll learn about Arrays.\n In the Arrays we can store number of elements of the same data type.\n Arrays are used to store multiple values in a single variable, instead of declaring separate variables for each value.\n To declare an Array, define the variable type, specify the name of the array followed by square brackets and specify the number of elements it should store.\n Let\'s store some values in an Array.\n";
    string Friends[3] = {"Sharandeep", "Harsharan", "Ritish"};
    cout<< Friends[0];
    cout<<"To access and change a element we can do \" arrayName[element number] = \"New Element\"; \" \n";
    cout<<"We can Loop through all the elements of an array, using for loop.\n Let's see.\n";
    for(int i = 0; i < 3; i++)
    {
      cout<<Friends[i] <<"\n";
    }
    cout<<"We can also output the elements with their indexes.\n";
    for(int i = 0; i < 3; i++)
    {
      cout<< i <<" : "<<Friends[i] <<"\n";
    }                                  
      
    /*
    #include<iostream>
using namespace std;
int main()
{
    bool ships[4][4] = {
        {0, 0, 0, 0},
        {1, 1, 1, 1},
        {0, 1, 0, 1},
        {0, 0, 1, 1}
    };
    int hits;
    int turns;
    
    while (hits < 4)
    {
        int row, column;
        cout<<"Selecting coordinates.\n";
        cout<<"Choose a row b/w 0 & 3 : ";
        cin>>row;
        cout<<"Choose a column b/w 0 & 3 :  ";
        cin>>column;
        
        if(ships[row][column])
        {
            ships[row][column] = 0;
            hits++;
            cout<<"Hit ! "<<(4-hits)<< " left.\n";
            
        }
        else
        {
            cout<<"Miss!\n\n";
        }
        turns++;
        
    }
     cout<<"You won !\n";
     cout<<"You took "<<turns<<" to win.\n";
     
     return 0;
    
}
    */
    
  
  return 0;
}
