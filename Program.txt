
using System;

namespace ReverseNumber
{
    class Program
    {
        static void Main(string[] args)
        {
            Console.WriteLine("Please type a numeric number"); 
            int number = int.Parse(Console.ReadLine());  
            int Reverse = 0; 
            while (number > 0) /// wish I was able to do some sort of input validation if someone tried to input letters, didn't even know where to start with that
            {
                int rem = number % 10; /// I had no idea of this equation, I needed help from a tech friend, couldn't take credit for it!
                number = number / 10;
                Reverse = (Reverse * 10) + rem;

            }
            Console.WriteLine("Reverse Number is " + Reverse);

            {
            }
        }
    }
}

