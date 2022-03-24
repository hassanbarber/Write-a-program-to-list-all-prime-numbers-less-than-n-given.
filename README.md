# Write-a-program-to-list-all-prime-numbers-less-than-n-given.
Write a program to list all prime numbers less than n given.
package bai05;
import java.util.Scanner;
public class Main {
 
     public static void lietKe(int n){
         System.out.print(" 2");
         for(int i=3;i<n;i+=2){
             if(cachamchung.checkSNT(i))System.out.print(" "+i);
         }
     }
     public static int enter(){
         Scanner input= new Scanner(System.in);
         boolean check= false;
         int n=0;
         while(!check){
             System.out.print(" ");
             try{
                 n= input.nextInt();
                 check= true;
             }catch(Exception e){
                 System.out.println("You must log in! or log in again...");
                 input.nextLine();
             }
         }
         return(n);
     }
     public static void main(String[] args) {
                 System.out.print("Tap n");
         int n= enter();
         System.out.println("Small numbers than "+n+ " ");
         lietKe(n);
     }
 
}
