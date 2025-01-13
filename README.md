# Java-Programs
Q1.Hello, World!: Write a Java program to print "Hello, World!" and ask the user for their name, then greet them.
import java.util.Scanner;

public class Greet {
    public static void main(String[] args) {
        System.out.println("Enter Your name");
        Scanner sc =new Scanner(System.in);
        String name = sc.nextLine();
        System.out.println("Hello World");
        System.out.println("Hello "+name);
    }
}


Q2.Simple Arithmetic: Create a program that takes two numbers as input and performs addition, subtraction, multiplication, and division.
import java.util.Scanner;

public class Arithmetic {
    public static void main(String[] args) {
        Scanner sc=new Scanner(System.in);
        System.out.println("Enter First Number");
        int a= sc.nextInt();
        System.out.println("Enter Second Number");
        int b=sc.nextInt();
        int sum=a+b;
        int mul=a*b;
        int sub=a-b;
        int div=a/b;
        System.out.println("The sum of both numbers is "+sum);
        System.out.println("The Multiplication of both numbers is "+mul);
        System.out.println("The substrsction of both numbers is"+sub);
        System.out.println("The divisioon of both numbers are "+div);
    }
}


Q3.Leap Year Checker: Write a program to determine if a given year is a leap year.
import java.util.Scanner;

public class Leapyearcheaker {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.println("Enter the year");
        int y=sc.nextInt();
        if((y%4==0 && y%100!=0)|| (y%400==0)){
            System.out.println(y+" is the leap year");
        }else{
            System.out.println(y+" is not a leap year");
        }
    }
}


Q4.Odd or Even: Develop a program to check if a number is odd or even using  conditional statements
import java.util.*;
public class Evenodd {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.println("Enter the number");
        int Num = sc.nextInt();

        if(Num%2==0){
            System.out.println("Given number is even");
        }
        else{
            System.out.println("The number is odd");
        }
    }
}


Q5.Sum of Digits: Write a Java program to calculate the sum of digits of a given number.
import java.util.Scanner;

public class SumOfDigits {
    public static void main(String[] args) {
        Scanner sc=new Scanner(System.in);
        System.out.println("Enter The Number");
        int n=sc.nextInt();
        int sum=0;
        while (n>0) {
            int temp =n%10;
            sum=sum + temp;
            n=n/10;
        }
        System.out.println("The Sum of the digits are "+sum);
    }
}
