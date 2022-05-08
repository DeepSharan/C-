# C++


#include<iostream>
#include<string>
#include<cmath>  
using namespace std;

class Fruits
{
    public: 
    string name;
    string color;
    int qty;
    
};
 
 class Bike
{
    public:
    string brand;
    string model;
    int year;
    
    Bike(string x, string y, int z)
    {
        brand = x;
        model = y;
        year = z;
    }
};   
  
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
  
  void fxn(string name, int age)
  {
    cout<<name<<" is "<<age<<" years old. \n\n";
  }
  
  int add(int x, int y)
  {
    return x + y;
  }
  
  void swap(int &x, int &y)
  {
    int z = x;
    x = y;
    y = z;
  }
  
   int sume(int k)
  {
      if (k > 0)
      {
          return k + sume(k - 1);
      }
      else
      {
          return 0;
      }   
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
      cout<<"Monday \n";
      break;
      case 2:
      cout<<"Tuesday \n";
      break;
      case 3:
      cout<<"Wednesday \n";
      break; 
      case 4:
      cout<<"Thursday \n";
      break;
      case 5:
      cout<<"Friday \n";
      break;
      case 6:
      cout<<"Saturday \n";
      break;
      case 7:
      cout<<"Sunday \n";
      break;
      default:
      cout<<"You are a fool :) \n";
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
    student2.rollNo = 22;
    
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
    
    cout<<"We can also use default parameters value, by using \"=\" operator. Like, if we call the function without any argument, it uses the default value.\n Inside a function, we can use as many parameters as we want, by separating them using comma.\n \n";
    
    fxn("Sharandeep", 21);
    
    cout<<"The void keyword indicates that the function does not return any value, but if you want your function to return any value, then use a data type (string, int, etc.), instead of void and use return keyword inside the function.\n";
    
    cout<< add(5, 10);
    
    cout<<"You can also store the results in a variable.";
    int z = add(5, 5);
    cout<< z <<"\n";
    cout<<"Now we will see swaping of numbers by storing reference value in the function, this can help changing the value of arguements.\n\n";
    
    int num1;
    cout<<"Input a number: ";
    cin >> num1;
    cout <<"Input another number: ";
    int num2;
    cin>> num2;
    
    cout<< "Before swap: \n";
    cout<<num1<<num2<<"\n";
    
    swap(num1, num2);
    
    cout<<"After swap: \n";
    cout<<num1<<num2<<"\n\n";
    
    cout<<"RECURSION, it is technique when function calls itself.\n\n";
    int result = sume(10);
    cout<< result <<"\n\n";
    
    cout<<"CLASSES, C++ is all about classes and objects, that contain both data and functions.\n We will see how to create classes and objects, but first we will learn what are classes and how they are used.\n";
    cout<<"Everything in C++ is associated with classes and objects, along with its attributes and methods.\n For example: in real life, a car is an object. The car has attributes, such as weight and color, and methods, such as drive and brake.\n\n Attributes and methods are variables and functions that belong to class, and are often referred as \'Class Members\'.\n A CLASS is user-defined data type that is often used as object constructor.\n\n To create a class use \'class\' keyword followed by class name, and start with curly braces, use the \'public\' keyword followed by colons, it is an access specifier, which specifies that the class members can be accessed from the outside the class, then start with writing the attributes of the class.\n\n";
    cout<<"Now we move on to creating the Objects.\n So, basically classes are templates for the objects, and the Objects are instances of Classes.\n When the Objects are created, they inherit all the variables and functions from the class.\n In C++, Object is created from a Class.\n\n To create an object of class, specify the \'className\' followed by \'ObjectName\'.";
    
    Fruits Obj1, Obj2;
    
    Obj1.name = "Mango";
    Obj1.color = "Yellow";
    Obj1.qty = 3;
    
    Obj2.name = "Banana";
    Obj2.color = "Red";
    Obj2.qty = 5;
    
    cout<<Obj1.qty<<" "<<Obj1.name<<" of "<<Obj1.color<<" colour.\n";
    cout<<Obj2.qty<<" "<<Obj2.name<<" of "<<Obj2.color<<" colour.\n\n";
    
    cout<<"CLASS METHODS - \n Basically, methods are functions that belongs to the class.\n We can also add parameters to the functions.\n There are two ways to define a function - \n 1. Inside the Class. \n 2. Outside the Class. \n First, we will see Function Inside the Class.";  
/*
    class Fruits
    {
      public: 
     
      void Method1()
      {
         cout<<"Gonna Execute ! \n";
      }
    };

    int main()
    {
      Fruits obj;
      obj.Method1();
    
      return 0;
    }
*/
    
    cout<<"Outside the Class.\n ";
/*
    class Fruits
    {
      public: 
     
       int Method2(int mango);

    };
    int Fruits::Method2(int mango)
    {
      return mango;
    }

    int main()
    {
      Fruits obj;
      cout<<obj.Method2(5);
    
      return 0;
    }
*/
    
    cout<<"CONSTRUCTORS \n A Constructor in C++ is a Special Method which is automatically called when an object is created.\n To create a class, same name is used followed by parentheses.\n The constructor has the same name as the class, it is always public, and it does not have any return value.\n Constructors can take parameters just like regular functions.\n";
/*
  class Bike
  {
    public:
    string brand;
    string model;
    int year;
    
    Bike(string x, string y, int z)
    {
        brand = x;
        model = y;
        year = z;
    }
   };
*/
   Bike object1("Yamaha", "R15", 2020);
   Bike object2("BMW", "Ace", 2019);
    
    cout<<object1.brand<<" "<<object1.model<<" "<<object1.year<<"\n";
    cout<<object2.brand<<" "<<object2.model<<" "<<object2.year<<"\n\n";
      
    cout<<"ACCESS SPECIFIER \n They define how the members of the Class can be accessed. \n These are three types - \n 1. public: \n 2. private: \n 3. protected: \n\n";
    cout<<"ENCAPSULATION \n The meaning of encapsulation is to ensure that the data is hidden from the users.\n To achieve this, you must keep the class members private & to access them use the public \"get\" and \"set\" methods.\n\n";
    /*
    class Emp
    {
      private:
      int salary;
    
      public:
      void setpay(int s)
      {
        salary = s;
      }
      int getpay()
      {
        return salary;
      }
    
    };
    int main()
    {
      Emp Deep;
      Deep.setpay(70000);
      Deep.getpay();
      cout<<"Salary of an Employee is "<<Deep.getpay()<<". \n\n";
    
      return 0;
     }
     */
     
     cout<<"INHERITANCE \n It is possible to inherit attributes and methods from one class to another using \':\' symbol.\n We group the inheritance concept into two categories: \n Parent Class. \t \t \t Child Class." ;
    /*
     class Vehicle
    {
      public:
      string brand;
      void honk()
      {
        cout<<"Pomm..Pomm !\n";
      }
    };
    class Car: public Vehicle
    {
      public:
      string model = "Cruze.";
    };
    int main()
    {
      Car car1;
      car1.brand = "Chevrolet";
      car1.honk();
    
      cout<<"My Car "<<car1.brand<<" "<<car1.model<<"\n";
    
     return 0;
     }          
     */                                                    
 
     cout<<"MULTILEVEL INHERITANCE \n In this, we can derive class from the other class, which is already derived from another class, with the same process of using \':\' symbol.\n";
     cout<<"MULTIPLE INHERITANCE \n In this, we can derive a class from more than one parent classes, just by separating them with comma.\n\n";    
     
     cout<<"POLYMORPHISM \n Polymorphism means \'many forms\' and it occurs when two or more classes are related to each other by inheritance.\n Polymorphism uses inherited methods to perform different tasks.\n This allows us to perform single action in different ways.\n\n";
      
      /*
      class Animals
      {
        public:
        void sound()
        {
           cout<<"Animals make the sound..\n";
        }
      };
      class Dog: public Animals
      {
        public:
        void sound()
        {
          cout<<"Dog barks - bow vow !\n";
        }
      };
      class Cat: public Animals
      {
        public:
        void sound()
        {
          cout<<"Cat - meow meow !\n";
        }
      };

      class Pig: public Animals
      {
        public:
        void sound()
        {
            cout<<"Pig - wee wee !\n";
        }
      };


      int main()
      {
        Animals myanimals;
        Dog mydog;
        Cat mycat;
        Pig mypig;
    
        myanimals.sound();
        mydog.sound();
        mycat.sound();
        mypig.sound();
    
        return 0;
      }
     */
      
      
      
  return 0;
}
