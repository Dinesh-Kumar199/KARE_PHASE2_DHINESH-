# KARE_PHASE2_DHINESH-
day 1 :
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
