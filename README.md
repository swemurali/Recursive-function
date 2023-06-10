# Recursive-function

## Aim:
To write a C# program to reverse a number using recursive function.

## Algorithm:
## Step1:
Create a function for reversing.

## Step2:
Get the number from the user.

## Step3:
In the function find reminder of the number and multiply it by 10 and add the reverse number.

## Step4:
Recusively call this function to get the reversed number.

## Step5:
print the reversed number.
## Program:
```
Developed by: Suwetha.M
Register Number: 212221230112

using System;
namespace Recursive
{
    class Program
    {
        public static int m, reverse = 0;
        public static int R(int n)
        {

            if (n > 0)
            {
                m = n % 10;
                reverse = reverse * 10 + m;
                n /= 10;
                return R(n);
            }
            return reverse;

        }
        static void Main(string[] args)
        {
            int num;
            Console.WriteLine("Enter a number:");
            num = Convert.ToInt32(Console.ReadLine());
            Console.WriteLine("Reverse of the number:");
            Console.WriteLine(R(num));
        }
    }
}
```
# #Output:

![244840469-6a0a3c01-9eb0-4e58-868c-3e0b9c4e84f4](https://github.com/swemurali/Recursive-function/assets/94165336/7f36d2fc-ffa1-4af5-8783-0694e07c5363)

## Result:
Thus the C# program to reverse a number using recursive function is executed successfully.
