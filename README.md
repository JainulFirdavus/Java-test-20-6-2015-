Please Answer the below questions briefly:


1.What is the most important feature of java?
-robust
-platform independent
-multithread
-secure


2.What do you mean by platform independent?
In Java the jvm automatically create the source code into machine code .
So the java will be platform independent it run all the operating system like Mac,Microsoft and Unix.

3.What is the difference between JVM,JDK and JRE?

JVM- Java Virtual Machine 
it is used to convert the source code into machine understandable code.

JDK- Java Development Kit
it has both jvm and jre in the same environment

JRE- Java Runtime Environment 

4.What is the concept called Pointers? And does java supports Pointer?

	Pointer it is used to save the variable  name in different address location.it is not that much of secure.
	So the java cannot be support the pointer . 	

5.What is the base class of all the classes?



6.What do you mean by local variables?

The local variable that initialized within the block or method. the local variable has no Default value.
once the block will end the value will destroy.

7.What do you mean by Class Variables?
 Class variable or Static Variable
 The static method call only the static variable
 that the static variable value will shared if you change the value and automatically all the chance on all location.

8.Can you explain: public static void main(String args[])

the public and static is the keyword that used the method will be "public". and "Static" the method will shared .
 "void" that return null value "main"  the main method of the java class.
 String args[]- all the operation can automatically converted into string. agrs[]- arguments 

9.Can main method to be overloaded?

no the main method can not be overloading we cannot put any parameter on the main method. 

10.Can a Class declared as protected?
no can initialized as protected class.



11.I don’t want my class to be inherited by other classes. What should I do?
"final" is the keyword used on the class we can't extended. 

12.What is the purpose of declaring variable as final?
 we declaring variable as final we cannot change the value .
 we can initialized the final variable at only once. 

13.What is the impact of declaring a method as final?
we can declare the method as final the method cannot be override.


14.What is an abstract class and what is the purpose?
The abstract keyword used for the class . that class must be extent. 
if a method using the abstract that the class will mention the abstract class. 

15.Can a abstract class defines as final?
No, we can't abstract class defines as final.
the final class cannot be extend .
but abstract class will deficiently class can extend.

16.Can you create object for abstract class?



17.What is the use of instanceof operator?
 the instanceof that used in if condition for the object can create for correct class.  

18.What is an abstract method?
the abstract method used in the class that the method will used on the base class.


19.What are the different types of if statements available?
simple if 
if else
if... elseif... elseif... else
nested if



20.Please explain about all access modifiers in java?
			|	same class	|	other class in same package |other class in other package 	|	other
public 		|		yes		|			yes					|		yes						| 	yes	
protected	|		yes		|			no					|		no						|	no
private		|		yes		|			yes					|		no						|	no
default		|		yes		|			yes					|		no						|	no



Please Write Programs for below scenario:

1.Getting three inputs from the user and displaying which one is greater one.

	import java.util.Scanner;
	 class main1
	{
		public static void main (String args[])
		{
			System.out.println("Enter the A B C Value ");
			Scanner in=new Scanner(System.in);
			System.out.println("enter the A Value:");
			int a = in.nextInt();
			System.out.println("enter the B Value:");
			int b = in.nextInt();
			System.out.println("enter the C Value:");
			int c = in.nextInt();

			if ((a>b)&&(a>c))
			{
				System.out.println("A is Greater");
			}
			else if ((b>a)&&(b>c))
			{
				System.out.println("B is Greater");
			}
			else if ((c>a)&&(c>b))
			{
				System.out.println("C is Greater");
			}
			else 
			
			System.out.println("All are equal");
			
			
			
			}
		
	}
			


2.Student Marks grade system.

import java.util.Scanner;

public class Grade 
{
    public static void main (String args[])
    {
        System.out.println("Enter the five subjects mark of the student ");
        Scanner in=new Scanner(System.in);
        System.out.println("Subject 1:");
        int m1 = in.nextInt();
        System.out.println("Subject 2:");
        int m2 = in.nextInt();
        System.out.println("Subject 3:");
        int m3 = in.nextInt();
        System.out.println("Subject 4: ");
        int m4 = in.nextInt();
        System.out.println("Subject 5:");
        int m5 = in.nextInt();
       
        if ((m1<45)||(m2<45)||(m3<45)||(m4<45)||(m5<45))  
        {
            System.out.println("Fail");
                    
        }
        else{
            
        
        int total=m1+m2+m3+m4+m5;        
        System.out.println("Total mark of the student is : "+total);
        int n=total/5;
        System.out.println("Average : "+n);

        if ((n>=80) && (n<=100))
        {
            System.out.println("grade A");
                       
        }
        else if ((n>=60) && (n<=80))
        {
            System.out.println("grade B");
                       
        }
        else if ((n>=50) && (n<=60))
        {
            System.out.println("grade C");
                       
        }
        else
        {
            System.out.println("grade D");
                       
        }
        } 
    
    }
    
            
}

3.sample program for abstract class and method concept?


a
abstract class A
{
abstract void display();
}

class B extends A
{
Void display()
{
System.out.println("hai i am abstract method");
}
}

class main1
{
public static void main(String args[])
{
A obj=new B();
obj.display();
}
}


4.Sample program for swapping two variables without using third variable?

import java.util.Scanner;
class swap
{

public static void main(String args[])
{

 System.out.println("Swap tw0 values");
 
Scanner in=new Scanner(System.in);
        System.out.println("value 1:");
        int a = in.nextInt();
		System.out.println("value 2:");
        int b = in.nextInt();
		a=a+b;
		b=a-b;
		a=a-b;
		System.out.println("value 1:"+a);
		System.out.println("value 2:"+b);
        
		
        
		
		
		

}

}


