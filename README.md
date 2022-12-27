# c-sharp-syntax-practice

## This is my first project, a calculator app, using and learning C# syntax. With this, I am also learning how to use Microsoft Visual Studio.

### First Line of Code.

```
            using System;
            using System.Collections.Generic;
            using System. Linq;
            using System. Text;
            using System.Threading.Tasks;

            namespace MyFirstPorject
            {
                class Program
                {
                    static void Main(string[] args)
                    {            
                        Console.WriteLine("Hello World"!); // WriteLine will print out a new line of text 
                        
                        Console.ReadLine();
                    }
                }
            }
```

### Drawing a Shape.

```
            Console.WriteLine("   /|");
            Console.WriteLine("  / |");
            Console.WriteLine(" /  |");
            Console.WriteLine("/___|");
            
            Console.ReadLine();
```

### Variables.

```
          string characterName = "Tom";
          int characterAge;
          characterAge = 30;
          
          Console.WriteLine("There once was a man named " + characterName);
          Console.WriteLine("He was " + characterAge + " years old");
          
          characterName = "Mike"
          characterAge = 40
          Console.WriteLine("He really liked the name " + characterName);
          Console.WriteLine("But didn't like being " + characterAge);
          
          Console.ReadLine();
```

### Data Types.

```
            string phrase = "Merry Christmas!");
            char grade = 'A';
            
            //int can be a negative value as well
            int age = 33;

            // float, double, decimal (from least accurate to very accurate like money)
            double gpa = 1.4;
            
            bool isFemale = true;
            
            Console.ReadLine();
```

### Working with Strings

```
            Console.WriteLine("Frances\"Fogarty");
            Console.WriteLine("Frances\nFogarty");
            
            string phrase = "Frances Fogarty" + "is cool"
            Console.WriteLine(phrase)
            
            string phrase = "Frances Fogarty" + "is cool"
            Console.WriteLine( phrase.Length );
            Console.WriteLine( phrase.ToUpper() );
            Console.WriteLine( phrase.Contains("fog") ); // returns true or false value
            Console.WriteLine( phrase[0]); // tells which character it contains on certain index
            Console.WriteLine( phrase.IndexOf("Frances") ); // which index position it starts, returns -1 if the char does not exist
            Console.WriteLine( phrase.Substring(8, 3) ); // returns "Fog"
            
            Console.ReadLine();
```

### Working with Numbers.

```
            Console.WriteLine( 20 );
            // mathematical operation ( + , - , * , / )
            // if you divide 2 int you always get a result of int ex. 5 / 2
            
            int num = 6;
            num++;
            Console.WriteLine( num ); // result is 7
            
            Console.WriteLine( Math.Abs(-40) ); // returns absolute number 40
            Console.WriteLine( Math.Pow(3, 2) ); // returns 9 (Power)
            Console.WriteLine( Math.Sqrt(36) ); // returns 6 (Square Root)
            Console.WriteLine( Math.Max(4, 90) ); // returns 90 (the biggest number between two numbers)
            Console.WriteLine( Math.Round(4.3) ); // returns 4
            Console.ReadLine();
```

### Getting User Input.

```
            Console.Write("Enter your name: "); // Write will just print out on the same line
            string name = Console.ReadLine(); // name is stored in the name variable
            Console.WriteLine("Hello " + name);
            Console.Write("Enter your age: "); 
            int age = Console.ReadLine();
            Console.WriteLine("Hello " + name + " you are " + age);
            Console.ReadLine(); // allowing us to see the output of our program on the console. it also pauses the execution of the program to allow user             input
```

### Building a Basic Calculator.

```
            int num = Convert.ToInt32("45"); // convert string to int
            Console.WriteLine(num + 6); // returns 51
            
            Console.Write("Enter a number: ");
            int num1 = Convert.toInt32( Console.ReadLine() ); // ReadLine always returns a string, so you need to convert it if using int
            Console.Write("Enter another number: ");
            int num2 = Convert.toInt32( Console.ReadLine() );
            
            Console.WriteLine(num1 + num2);
            
            Console.Write("Enter a number: ");
            double num1 = Convert.ToDouble( Console.ReadLine() ); // ToDouble handles decimals
            Console.Write("Enter another number: ");
            double num2 = Convert.ToDoouble( Console.ReadLine() );
            
            Console.WriteLine(num1 + num2);
            
            Console.ReadLine();
```

### Building a Simple Mad Lib Game.

```
            string color, pluralNoun, celebrity; // declare all variables then give values
            Console.Write("Enter a color: ")
            string color = Console.ReadLine();
            Console.Write("Enter a plural noun: ");
            string pluralNoun = Console.ReadLine();
            Console.Write("Enter a celebrity: ");
            string celebrity = Console.ReadLine();
            
            Console.WriteLine("Roses are " + color);
            Console.WriteLine(pluralNoun + " are blue");
            Console.WriteLine("I Love " + celebrity);
            
            Console.ReadLine();
```

### Arrays.

```
            int[] luckyNumbers = { 4, 8, 15, 48, 32 };

            luckyNumbers[0] = 7;

            Console.WriteLine(luckyNumbers[0]);

            Console.ReadLine();

```

```
            string[] friends = new string[3];

            friends[0] = "Matt";
            friends[1] = "Frances";

```

### Methods.

```
            class Program
            {
                        static void Main(string[] args)
                        {
                            SayHi("Frances", 33); // Call the method from down below
                            SayHi("Matthew", 34);
                            
                            Console.ReadLine();       
                        }
                        
                        static void SayHi(string name, int age) // methods accept parameters
                        {
                            Console.WriteLine("Hello " + name + " you are " + age);
                        }
            }
```

### Return Statement.

```
            class Program 
            {
                        static void Main(string[] args)
                        {
                                    Console.WriteLine( cube(5) );
                                    Console.ReadLine();
                        }
                        
                        static int cube(int num)
                        {
                                    int result = num * num * num;
                                    return result // return is a special keyword
                        }
            }
```


### If Statements.

```
            bool isFemale = true;
            bool isTall = true;
            
            if (isFemale && isTall)
            {
                        Console.WriteLine("You are tall female");
            } else if (isFemale && !isTall)
            {
                        Console.WriteLine("You are a short female")
            } else if (!isFemale && isTall)
            {
                        Console.WriteLine("You are not a female but you are tall")
            } else
            {
                        Console.WriteLine("You are not female and not tall");
            }
            
            Console.ReadLine();
```

### If Statements (comparisons).

```
            
                    class Program 
            {
                        static void Main(string[] args)
                        {
                                    Console.WriteLine( GetMax(2, 10, 6) );
                                    Console.ReadLine();
                        }
                        
                        static int GetMax(int num1, int num2, int num3)
                        {
                                int result;
                                
                                if (num1 >= num2 && num1 >= 3)
                                {
                                    result = num1;
                                } else if (num2 >= num1 && num2 >=3)
                                {
                                    result = num2;
                                } else
                                {
                                    result = num3;
                                }
                                
                                return result;
                        }
            }
```

### Building a Better Calculator.

```
            class Program 
            {
                        static void Main(string[] args)
                        {
                                    Console.Write("Enter a number: ");
                                    double num1 = Convert.ToDouble( Console.ReadLine() );
                                    
                                    Console.Write("Enter Operator: ");
                                    string op = Console.ReadLine();
                                    
                                    Console.Write("Enter another number: ");
                                    double num2 = Convert.ToDouble( Console.ReadLine() );
                                    
                                    if (op === "+")
                                    {
                                                Console.WriteLine(num1 + num2);
                                    } else if (op === "-")
                                    {
                                                Console.WriteLine(num1 - num2);
                                    } else if (op === "*")
                                    {
                                                Console.WriteLine(num1 * num2);
                                    } else if (op === "/")
                                    {
                                                Console.WriteLine(num1 / num2);
                                    } else
                                    {
                                                Console.WriteLine("Invalid Operator");
                                    }
                                    
                                    Console.ReadLine();
                        }
            }
```

### Switch Statements.

```
            class Program 
            {
                        static void Main(string[] args)
                        {
                                    Console.WriteLine( GetDay(0) );
                                    Console.ReadLine();
                        }
                        
                        static string GetDay(int dayNum)
                        {
                                    string dayName;
                                    
                                    switch (dayNum)
                                    {
                                                case 0: 
                                                            dayName = "Sunday";
                                                            break;
                                                case 1:
                                                            dayName = "Monday";
                                                            break;
                                                case 2:
                                                            dayName = "Tuesday";
                                                            break;
                                                case 3:
                                                            dayName = "Wednesday";
                                                            break;
                                                case 4:
                                                            dayName = "Thursday";
                                                            break;
                                                case 5:
                                                            dayName = "Friday";
                                                            break;    
                                                case 6:
                                                            dayName = "Saturday";
                                                            break;
                                                default:
                                                            dayName = "Invalid Day Number";
                                                            break;
                                    }
                                    
                                    return dayName;
                        }
            } 
```

### While Loops.

```
            class Program 
            {
                        static void Main(string[] args)
                        {
                                    int index = 1;
                                    while (index <= 5) // as long as this condition is true, it will keep looping
                                    {
                                                Console.WriteLine(index);
                                                index++;
                                    }
                                    
                                    Console.ReadLine();
                                    
                                    // Do While Loop
                                    int index = 6;
                                    do
                                    {
                                                Console.WriteLine(index);
                                                index++;
                                    } while (index <= 5);
                                    
                                    Console.ReadLine();
                        }
            }
```

### Building a Guessing Game.

```

```
