# hello_world

using System;

namespace Simple
{
    public class Program
    {
        public static void Main(string[] args)
        {
            int num = 7;
            string line = "-";
            string star = "*";

            //first row
            for (int i = 0; i < 2; i++)
            {
                for (int s = 0; s < num * 5; s++)
                {
                    if (s >= 0 && s < num | s >= num * 2 && s < num * 3 | s >= num * 4 && s < num * 5)
                    {
                        Console.Write(line);
                    }

                    else 
                    {
                        Console.Write(star);
                    }
                }

            }
            Console.WriteLine();

            //second row
            for (int i = 0; i < 2; i++)
            {
                for (int s = 0; s < num * 5; s++)
                {
                    if (s >= 0 && s < num - 1 | s >= num * 2 + 1 && s < num * 3 - 1 | s >= num * 4 + 1 && s < num * 5)
                    {
                        Console.Write(line);
                    }

                    else 
                    {
                        Console.Write(star);
                    }
                }
            }
            Console.WriteLine();

            //third row
            for (int i = 0; i < 2; i++)
            {
                for (int s = 0; s < num * 5; s++)
                {
                    if (s == 0 || s == num + 1 || s == num * 3+1||s==num*5-1)
                    {
                        Console.Write(line);
                    }

                    else 
                    {
                        Console.Write(star);
                    }
                }              
                               
            }
            Console.WriteLine();

            //fourth row

            for (int i = 0; i < 2; i++)
            {
                for (int s = 0; s < num * 5; s++)
                {
                    
                    if (s >= 0 && s < num | s >= num * 2 && s < num * 3||s>=num*4&& s<num*5)
                    {
                        Console.Write(star);
                    }
                    else 
                        Console.Write(line);
                }

            }
            Console.WriteLine();


            Console.ReadKey();
        }
    }
}
