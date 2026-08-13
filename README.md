# KARE_PHASE2_DHINESH-
day 1:
   public class Main{
        public static void main(String[]args){
            System.out.println("cse\"KARE\"Students");
        }
    }
        public class Main{
        public static void main(String[]args){
            System.out.print("\\n");
    }
}

    public class Main{
        public static void main(String[]args){
          if(true)
          System.out.println("hi");
          else
          System.out.println("Hello");
    }
}
    public class Main{
        public static void main(String[]args){
          int a = 3;
          if(a==4)
          System.out.println(a-5);
          else
          System.out.println(a+8);
        }
}
    public class Main{
        public static void main(String[]args){
          if(2+2==4)
         System.out.println("Welcome");
         else{
             System.out.println("Update your details");
         }
      }
    }
PALINDROME NUMBER
import java.util.*;
class Main{
    public static void main(String[] args){
        Scanner obj = new Scanner(System.in);
        int n = obj.nextInt();
        int temp = n,d,rev=0;
        while(n!=0){
            d=n%10;
            rev = rev * 10 + d;
            n = n/10;
        }
        if(temp == rev)
        System.out.println("palindrome nmber");
        else
        System.out.println("Not a palindrome number ");
    }
}

import java.util.Scanner;

public class Main {

    static int reverse(int n) {
        int rev = 0;
        while (n > 0) {
            rev = rev * 10 + (n % 10);
            n /= 10;
        }
        return rev;
    }

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        System.out.print("Enter a number: ");
        int n = sc.nextInt();

        int square = n * n;
        int rev = reverse(n);
        int revSquare = rev * rev;
        int revRevSquare = reverse(revSquare);

        if (square == revRevSquare)
            System.out.println(n + " is an Adam Number.");
        else
            System.out.println(n + " is NOT an Adam Number.");

        sc.close();
    }
}
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        System.out.print("Enter the starting number: ");
        int start = sc.nextInt();

        System.out.print("Enter the ending number: ");
        int end = sc.nextInt();

        System.out.println("Prime numbers between " + start + " and " + end + " are:");

        for (int i = start; i <= end; i++) {
            if (i < 2)
                continue;

            boolean isPrime = true;

            for (int j = 2; j <= Math.sqrt(i); j++) {
                if (i % j == 0) {
                    isPrime = false;
                    break;
                }
            }

            if (isPrime) {
                System.out.print(i + " ");
            }
        }

        sc.close();
    }
}
//reverse number
import java.util.*;
class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n=sc.nextInt();
        int d,ans=0;
        while(n!=0)//4
        {
            d=n%10;//4%10=4
            ans=ans*10+d;//65*10+4=654
            n=n/10;//4/10=0
        }
        System.out.println("Reverse Number:"+ans);
    }
}

//to count no of digits in the given Number
//logic- n=4862
//        486 c=1
//         48 c=2 
//          4 c=3
//          0 c=4 
import java.util.*;
class Main {
    public static void main(String[] args){
        Scanner obj=new Scanner(System.in);
        int n=obj.nextInt();
        int c=0;
        while(n!=0) 
        {
            n=n/10;
            c++;
        }
            System.out.print(" No of digits:"+c);
        
    }
}

//to count the odd even digits in the given Number
//i/p                              o/p 
//4821                             Odd digit count:1 
//                                 Even digit count:3
import java.util.*;
class Main {
    public static void main(String[] args) {
        Scanner obj = new Scanner(System.in);
        int n = obj.nextInt();
        int ec=0,oc=0,d;
        while(n!=0)
        {
            d=n%10;
            if(d%2==0)
            ec++;
            else 
            oc++;
            n=n/10;
        }
        System.out.println("Odd digit count:"+oc);
        System.out.println("Odd digit count:"+ec);
    }
}

//to count the prime digits in the given Number

import java.util.*;
class Main {
    public static void main(String[] args) {
        Scanner obj = new Scanner(System.in);
        int n = obj.nextInt();
        int c=0,d;
        while(n!=0)
        {
            d=n%10;
            if(d==2||d==3||d==5||d==7)
            c++;
            n=n/10;
        }
        System.out.println("Prime digit count:"+c);
    }
}

//to reverse the given Number without using right side formation

import java.util.*;
class Main {
    public static void main(String[] args) {
        Scanner obj = new Scanner(System.in);
        int n = obj.nextInt();
        int d;
        while(n!=0)
        {
            d=n%10;
            System.out.print(d);
            n=n/10;
        }
    }
}

//palindrome number

import java.util.*;
class Main {
    public static void main(String[] args) {
        Scanner obj = new Scanner(System.in);
        int n = obj.nextInt();
        int temp = n;
        int d,ans=0;
        while(n!=0)
        {
            d=n%10;
            ans=ans*10+d;
            n=n/10;
        }
        if(temp==ans)
        System.out.println("Palindrome Number");
        else
        System.out.println("Not a Palindrome Number");
    }
}
//base 2 pattern
import java.util.*;
public class Main {
    public static void main(String[] args) {
        int i,row,col;
        Scanner obj = new Scanner(System.in);
        int n = obj.nextInt();
        for(row=0;row<n;row++,System.out.println()) {
            for(col=0;col<=row;col++)
            System.out.print("*");
        }
    }
}
//base 3 pattern
import java.util.*;
public class Main {
    public static void main(String[] args) {
        int i,row,col;
        Scanner obj = new Scanner(System.in);
        int n = obj.nextInt();
        for(row=0;row<n;row++,System.out.println()) {
            for(col=0;col<n-row;col++)
            System.out.print("*");
        }
    }
}
//base 4 pattern
import java.util.*;
public class Main {
    public static void main(String[] args) {
        int i,row,col;
        Scanner obj = new Scanner(System.in);
        int n = obj.nextInt();
        for(row=0;row<n;row++,System.out.println()) {
            for(col=0;col<2*row-1;col++)
            System.out.print("*");
        }
    }
}
//base 3+1 pattern
import java.util.*;
public class Main {
    public static void main(String[] args) {
        int i,row,col;
        Scanner obj = new Scanner(System.in);
        int n = obj.nextInt();
        for(row=0;row<n;row++,System.out.println()) {
            for(col=0;col<n-row-1;col++)
            System.out.print(" ");
            for(col=0;col<n;col++)
            System.out.print("*");
        }
    }
} 
//base 2+1 pattern
import java.util.*;
public class Main {
    public static void main(String[] args) {
        int i,row,col;
        Scanner obj = new Scanner(System.in);
        int n = obj.nextInt();
        for(row=0;row<n;row++,System.out.println()) {
            for(col=0;col<=row-1;col++)
            System.out.print(" ");
            for(col=0;col<=n;col++)
            System.out.print("*");
        }
    }
} 
//base 2+3+2 pattern
import java.util.*;
public class Main {
    public static void main(String[] args) {
        int i,row,col;
        Scanner obj = new Scanner(System.in);
        int n = obj.nextInt();
        for(row=0;row<n;row++,System.out.println()) {
            for(col=0;col<=row;col++)
            System.out.print("*");
            for(col=0;col<n-row-1;col++)
            System.out.print(" ");
            for(col=0;col<=row;col++)
            System.out.print("*");
        }
    }
} 
//base 2+3+3+2 pattern
import java.util.*;
public class Main {
    public static void main(String[] args) {
        int i,row,col;
        Scanner obj = new Scanner(System.in);
        int n = obj.nextInt();
        for(row=0;row<n;row++,System.out.println()) {
            for(col=0;col<=row;col++)
            System.out.print("*");
            for(col=0;col<n-row-1;col++)
            System.out.print(" ");
            for(col=0;col<n-row-1;col++)
            System.out.print(" ");
            for(col=0;col<=row;col++)
            System.out.print("*");
        }
    }
} 
//base 2+ 3 
import java.util.*;
public class Main {
    public static void main(String[] args) {
        int i,row,col;
        Scanner obj = new Scanner(System.in);
        int n = obj.nextInt();
        for(row=0;row<n-1;row++,System.out.println()) {
            for(col=0;col<=row;col++)
            System.out.print("*");
        }
        for(row=0;row<n;row++,System.out.println()) {
            for(col=0;col<n-row;col++)
            System.out.print("*");
        }    
    }
} 
//butterfly
import java.util.*;
public class Main {
    public static void main(String[] args) {
        int i,row,col;
        Scanner obj = new Scanner(System.in);
        int n = obj.nextInt();
        for(row=0;row<n-1;row++,System.out.println()) {
            for(col=0;col<=row;col++)
            System.out.print("*");
            for(col=0;col<n-row-1;col++)
            System.out.print(" ");
            for(col=0;col<n-row-1;col++)
            System.out.print(" ");
            for(col=0;col<=row;col++)
            System.out.print("*");
        }
        for(row=0;row<n;row++,System.out.println()) {
            for(col=0;col<n-row;col++)
            System.out.print("*");
            for(col=0;col<=row-1;col++)
            System.out.print(" ");
            for(col=0;col<=row-1;col++)
            System.out.print(" ");
            for(col=0;col<n-row;col++)
            System.out.print("*");
        }    
    }
}

//switch
import java.util.Scanner;
class Main{
    public static void main(String[] args){
        Scanner obj = new Scanner(System.in);
        int n = obj.nextInt();
        switch(n)
        {
            case 1:
                System.out.print("CSE");
                break;
            case 2:
                 System.out.print("ECE");
                 break;
            case 3:
                System.out.print("EEE");
                break;
                default:
                System.out.print("Invalid input");
        }
    }
}
//1
class Main {
    public static void main(String[] args) {
        if(true)
        System.out.print("Hi");
        else
        System.out.print("Hello");       
    }
}
//2
class Main {
    public static void main(String[] args) {
        int a = 3;
        if(a==4)
        System.out.print(a+5);
        else
        System.out.print(a-8);
    }
}
//3
class Main {
    public static void main(String[] args) {
        if(2+2==4)
        System.out.print("Welcome");
        ///System.out.print("Update your details");
        else
        System.out.print("Thank you");
    }
}
//4
class Main {
    public static void main(String[] args) {
        if(!true)
        System.out.print(2+3*5);
        else
        System.out.print(5*6/2+10);
    }
}
//5
class Main {
    public static void main(String[] args) {
        int a = 11;
        int b = a--;
        int x = 40;
        int y = x++;
        System.out.print(a+" "+b+" "+x+" "+y);
    }
}
//6
class Main {
    public static void main(String[] args) {
        int a = 29;
        int b = a++;
        int c = --b;
        int d = c++;
        int e = ++d;
        System.out.print(a+" "+b+" "+c+" "+d+" "+e);
    }
}
//7
class Main {
    public static void main(String[] args) {
        int a = 99;
        int b = a++;
        int c = b--;
        int d = --c;
        int e = d++;
        int f = e--;
        System.out.println(f++);
        System.out.println(a+" "+b+" "+c+" "+d+" "+e+" "+f);
    }
}
//8
import java.util.Scanner;
public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.print("Enter a number:");
        int num = sc.nextInt();
        if (num%2 == 0){
            System.out.println(num+ "is even");
        }
        else {
            System.out.println(num+ " is odd");
        }
    }
}
