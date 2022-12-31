//Find Prime Number
import java.util.Scanner;
public class Main{
    public static void main(String[] args){
        Scanner input = new Scanner(System.in);
        System.out.print("enter a number :");
        int n = input.nextInt();
        boolean isPrime = true;
        for(int i = 2; i<=n/2 ; i++){
            if(n%i==0)
                isPrime = false;
            break;
        }
        if ( isPrime)
            System.out.println(n + " is prime");
        else
            System.out.println(n + " it is not prime");
    }
}
