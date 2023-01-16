# c-sharp-syntax-practice

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
            class Program 
            {
                        static void Main(string[] args)
                        {
                                    string secretWord = "family";
                                    string guess = "";
                                    int guessCount = 0;
                                    int guessLimit = 3;
                                    bool outOfGuesses = false;
                                    
                                    while (guess != secretWord && !outOfGuesses)
                                    {
                                                if (guessCount < guessLimit)
                                                {
                                                            Console.Write("Enter guess: ");
                                                            guess = Console.ReadLine();
                                                            guessCount++;
                                                } else
                                                {
                                                            outOfGuesses = true;
                                                }

                                    }
                                    
                                    if (outOfGuesses)
                                    {
                                                Console.Write("You Lose!");
                                    } else
                                    {
                                                Console.Write("You Win!");
                                    }

                              
                                    Console.ReadLine();
                        }
                        
                        static int cube(int num)
                        {
                        }
            }
            
```

### For Loops.

```
               class Program 
            {
                        static void Main(string[] args)
                        {
                                    int i = 1;
                                    while (i <= 5)
                                    {
                                                Console.WriteLine(i);
                                                i++;
                                    }
                                    
                                    for( int i = 1;  i <= 5; i++ )
                                    {
                                                Console.WriteLine(i);
                                    }
                                    
                                    Console.ReadLine();
                        }
            }         
```
```
               class Program 
            {
                        static void Main(string[] args)
                        {
                                    int[] luckyNumbers = { 4, 8, 16, 44, 48, 88 };
                                    for (int i = 0; i < luckyNumbers.Length; i++)
                                    {
                                                Console.WriteLine( luckyNumber(i) );
                                    }
                        }
            }   
```

### Building an Exponent Method.

```
            class Program 
            {
                        static void Main(string[] args)
                        {
                                    Console.WriteLine( GetPow(3, 2) );
                                    Console.ReadLine();
                        }
                        
                        static int GetPow(int baseNum, int powNum)
                        {
                                    int result = 1;
                                    
                                    for(int i = 0; i < powNum; i++)
                                    {
                                                result = result * baseNum;
                                    }
                                    
                                    return result;
                        }
            }   
```

### 2D Arrays.

```
            class Program 
            {
                        static void Main(string[] args)
                        {
                                    int[,] numberGrid = { 
                                      { 1, 2 },
                                      { 3, 4 },
                                      { 5, 6 },
                                    };
                                    
                                    int[,] = new myArray[2, 3];
                                    
                                    Console.WriteLine(numberGrid[0, 0]); // returns 1, [1, 1] returns 4
                                    
                                    Console.ReadLine();
                        }
            }  
```

### Comments.

```
            This is how you write a comment in C#:
            
            // This is a single line comment. 
            /* This is how 
            to write 
            a comment 
            with multiple 
            lines. */
```

### Exception Handling.

```
            // Exception handling is simply catching exception, in JS it's called "Error Handling"
            // Try Catch block
            
            try
            {
                        Console.Write("Enter a number: ");
                        int num1 = Convert.ToInt32(Console.ReadLine());
                        Console.Write("Enter another number: ");
                        int num2 = Convert.ToInt32(Console.ReadLine());
            
                        Console.WriteLine(num1 / num2);
            }
            catch (DivideByZeroException e) // you can specify an exception and will only catch that exception
            {
                        Console.WriteLine(e.Message);
            }
            catch (FormatException e)
            {
                        Console.WriteLine(e.Message);
            }
            finally 
            {
                        // all the code in this block will always be executed       
            }

            // default: catch (Exception e) {}
            // Check out C# exception list
            
            Console.ReadLine();
```

### Classes & Objects / Constructors.

```
            Book.cs
            class Book 
            {
                                    // Objects & Classes allows to create own custom data types
                                    // A Class is just a specification for a new data type or blue print and used to model real world entities to be used in the program
                                    
                                    public string title;
                                    public string author;
                                    public int pages;
                                    
                                    public Book(string aTitle, string aAuthor, int aPages) // The Constructor inside of a class
                                    {
                                                title = aTitle;
                                                author = aAuthor;
                                                pages = aPages;
                                    }
            }  
            
            Program.cs
            class Program 
            {
                        static void Main(string[] args)
                        {
                                    // Object is an instance of a class
                                    Book book1 = new Book("Harry Potter", "JK Rowling", 400);
                                    
                                    Book book2 = new Book("Lord of the Rings", "Tolkein", 700);;
                                    
                                    Console.WriteLine(book2.title);
                                    
                                    Console.ReadLine();
                        }
            }  
            
```

### Object Methods.

```
            // In Student.cs
            class Student
            {
                        public string name;
                        public string major;
                        public double gpa;
                        
                        public Student(string aName, string aMajor, double aGpa)
                        {
                                    name = aName;
                                    major = aMajor;
                                    gpa = aGpa;
                        }
                        
                        public bool HasHonors()
                        {
                                    if (gpa >= 3.5)
                                    {
                                                return true;
                                    }
                                    return false;
                        }
            }
            
            // In Program.cs
            class Program 
            {
                        static void Main(string[] args)
                        {
                                    Student student1 = new Student("Jim", "Business", 2.8);
                                    Student student1 = new Student("Pam", "Art", 3.6);
                                    
                                    Console.WriteLine( student1.HasHonors() ); // return false
                                    Console.WriteLine( student2.HasHonors() ); // return true
                                    
                                    Console.ReadLine();
                        }
            }  
```

### Getters and Setters.

```
            // In Movie.cs
            class Movie
            {
                        public string title;
                        public string director;
                        private string rating; // Only code in the movie class can access this
                        
                        public Movie(string aTitle, string aDirector, string aRating);
                        {
                                    title = aTitle;
                                    director = aDirector;
                                    rating = aRating;
                        }
                        
                        public string Rating
                        {
                                    get 
                                    { 
                                                return rating; 
                                    }
                                    set 
                                    { 
                                                if (value == "G" || value == "PG" || value == "PG-13" || value == "R" || value == || "NR")
                                                {
                                                            rating = value;
                                                } else {
                                                            rating = "NR";
                                                }
                                    }
                        }
            }
            
            // In Program.cs
            class Program 
            {
                        static void Main(string[] args)
                        {
                                    Movie avengers = new Movie("The Avengers", "Joss Whedon", "PG-13");
                                    Movie shrek = new Movie("Shrek", "Adam Adamson", "PG");
                                    
                                    Console.ReadLine();
                        }
            }     
```

### Static Class.

```
            // In Song.cs
            class Song
            {
                        public string title;
                        public string artist;
                        private int duration;
                        public static int songCount = 0; // static attribute which belongs to the Class Song
                        
                        public Movie(string aTitle, string aArtist, string aDuration);
                        {
                                    title = aTitle;
                                    artist = aArtist;
                                    duration = aDuration;
                                    songCount++;
                        }
            }
            
            // In Program.cs
            class Program 
            {
                        static void Main(string[] args)
                        {
                                    Song holiday = new Song("Holiday", "Green Day", 200);
                                    Console.WriteLine(Song.songCount); // giving info about the class in general not a secific object
                                    Song kashmir = new Song("Kashmir", "Led Zeppelin", 150);
                                    Console.WriteLine(Song.songCount); // giving info about the class in general not a secific object
                                    
                                    Console.ReadLine();
                        }
            }    
```

### Static Methods & Classes.

```
            // In Porgram.cs
            class Program
            {
                        static void Main(string[] args)
                        {
                                    Console.WriteLine(Math.Sqrt(144)); // static methods is not having to create an instance, a method that belongs to a class
                                    
                                    UsefulTools.SayHi("Frances");
                                    
                                    Console.ReadLine();
                        }
            }
            
            // In UsefulTools.cs
            
            class UsefulTools
            {
                        public static void SayHi(string name)
                        {
                                    Console.WriteLine("Hello" + name);
                        }
            }
```

### Inheritance.

```
            // Inheritance is basically a technique that can be used in C# where we can have a sub class inherit all the functionality of super class
            
            // In Porgram.cs
            class Program
            {
                        static void Main(string[] args)
                        {
                                    Chef chef = new Chef();
                                    chef.MakeChicken();
                                    
                                    ItalianChef chef = new ItalianChef();
                                    italianChef.MakeChicken();
                                    
                                    Console.ReadLine();
                        }
            }
            
            // In Chef.cs
            class Chef
            {
                        public void MakeChicken()
                        {
                                    Console.WriteLine("The Chef makes chicken");
                        }
                        
                        public void MakeSalad()
                        {
                                    Console.WriteLine("The Chef makes salad");
                        }
                        
                        public virtual void MakeSpecialDish() 
                        // virtual - this method can be overriden in any sub classes
                        // subclasses can change the functionality of this method
                        {
                                    Console.WriteLine("The Chef makes bbq ribs");
                        }
            }
            
            // In ItalianChef.cs
            class ItalianChef : Chef // the ItalianChef is going to inherit all functionalities the Chef has
            {
                        public override void MakeSpecialDish() // keyword - override
                        {
                                    Console.WriteLine("The Chef makes chicken parm");
                        }
                        
                        public void MakePasta()
                        {
                                    Console.Write("The Chef makes pasta");
                        }
            }
```
