# C++


#include<iostream>
#include<string>
#include<cmath>  
using namespace std;
  
  struct specs
    {
      string Brand ;
      string Model ;
      int year ;
    };
  void intake(string name)
  {
    cout<<"Hello "<<name<<"\n";
  }
  
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
    cout<<"Now we\'ll see how to create and use Structures(struct).\n To create structures we use \"struct\" keyword, and declare each of its member inside curly braces.\n To access the members of structure we use dot(.) syntax.\n We can use one structure for multiple variables using commas.\n We can name the structure and use them as data types.\n Firstly, we will see one structure in multiple variables.\n ";
    struct 
    {
      string name;
      int rollNo ;
    } 
    student1, student2, student3;
    
    student1.name = "Sharandeep";
    student1.rollNo = 21;
    
    student2.name = "Harsharan";
    student2.rollNo. = 22;
    
    student3.name = "Ritish";
    student3.rollNo = 23;
    
    cout<<student1.name<<" "<<student1.rollNo<<"\n";
    cout<<student2.name<<" "<<student2.rollNo<<"\n";
    cout<<student3.name<<" "<<student3.rollNo<<"\n\n";
    
    cout<<"Now, we\'ll see the named structures.\n REMEMBER, whenever we want to use structures as data type, we need to declare them before main funcion i.e. before the int main(). \n";
    
    specs car1, car2, car3;
    car1.Brand = "BMW";
    car1.Model = "X8";
    car1.year = 2018;
    
    car2.Brand = "Mercedes";
    car2.Model = "A6";
    car2.year = 2019;
    
    car3.Brand = "Audi";
    car3.Model = "R8";
    car3.year = 2020;
    
    cout<<car1.Brand<<" "<<car1.Model<<" \n";
    cout<<car2.Brand<<" "<<car2.Model<<" \n";
    cout<<car3.Brand<<" "<<car3.Model<<" \n\n";
    
    cout<<" \"References\" variable is reference to an existing variable, declared by & operator.\n";
    string food = "Burger";
    string &meal = food;
    cout<<"Either we can use food or meal to output burger. \n";
    cout<<food<<" \n";
    cout<<meal<<"\n\n";
    
    cout<<"& Operator can also be used to get the memory address of the variable, i.e. which is the location of where the variable is stored on computer.\n";
    cout<< &food<<"\n\n";
    
    cout<<"Pointers store the memory address as its value.";
    
    string *ptr = &food;
    cout<< ptr<<"\n\n";
    cout<<"Remember, * can be confusing.\n As, when \" * \" used in declaration, it creates pointer variable.\n When not used in declaration, it acts as dereference operator. \n\n As we see below: \n";
    cout<< *ptr<<"\n";
    cout<<"Modify pointers: \n";
    *ptr = "Pizza";
    cout<< *ptr <<"\n";
    cout<< food <<"\n\n";
    
    cout<<"We\'ll learn about the C++ functions. \n\n";
    cout<<" To declare a function, specify function name followed by parenthesis(), \n for example- void functionName(){ code to be executed } \n We will see further about creating functions.\n\n";
    cout<<"Declared functions are not used immediately, they are saved for later use, they are executed when they are called.\n To call a function, write the function name followed by parenthesis and a semicolon.\n";
    cout<<"C++ function consists of two parts: Declaration & Definition. \n Declaration is always before the main function, but definition can be done below the main function.\n They can be declared and defined together, but it is possible to separate them for code optimisation.\n Declaration : the return type, the name of the function, and parameters(if any) \n Definition : the body of function(code to be executed). \n\n";
    cout<<"Info can be passed to the function as parameters. Parameters act as variables, and are declared in parenthesis. \n";
    
    intake("Sharandeep");
    
    
    
        
      
      
    
  
  return 0;
}
