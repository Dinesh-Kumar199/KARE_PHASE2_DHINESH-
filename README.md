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
