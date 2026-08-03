# KARE_PHASE2_DHINESH-
day 1 :
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
