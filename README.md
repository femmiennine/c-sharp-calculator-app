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
                        Console.WriteLine("Hello World"!);
                        
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
          Console.WriteLine("He really liked the name " + characterName);
          Console.WriteLine("But didn't like being " + characterAge);
          
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
