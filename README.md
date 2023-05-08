# Operator-Overloading

## Aim:
 To write a C# program to pass values through constructors(default and parameterized) and also overload equal operators by checking whether objects are equal using operator overloading. 
 
 ## Algorithm:
 ### Step 1:
Create a class for operator overloading.

### Step 2:
Get inputs for length,breadth from the user in overloading function.

### Step 3:
Compare the inputs such as length and breadth.

### Step 4:
Using equal to(==) and not equal to(!=) operator we can compare the inputs.

### Step 5:
After that print the result.
 
 
 
 ## Program:
 ```
 Developed by :Shobika P
 Register No:212221230096

 using System;
class program
{
    public program()
    {
        Console.WriteLine("Default Constructor");
    }
    public program(int number)
    {
        Console.WriteLine(number);
    }
    public static bool operator == (program p1,program p2)
    {
        return p1.Equals(p2);
    }
    public static bool operator != (program p1, program p2)
    {
        return !p1.Equals(p2);

    }
}
class Example
{
    public static void Main()
    {
        program p1 = new program();
        program p2 = new program(10);
        if(p1==p2)
        {
            Console.WriteLine("Objects are equal");

        }
        else
        {
            Console.WriteLine("Objects are not equal");

        }

    }
}
 ```
 
 
 ## Output:
 ![Screenshot (28)](https://user-images.githubusercontent.com/94508142/236787400-4c82987d-8f21-4678-9964-0480e3dd7e6e.png)
 ![Screenshot (30)](https://user-images.githubusercontent.com/94508142/236788208-17a0bb94-4954-4779-add4-893c46f2760e.png)


 
 
 ## Result:
 Thus the C# program to find the volume of a box using operator overloading is implemented successfully.
