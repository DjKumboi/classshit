# classshit
forgot usb
public class indefiniteloops{
public static void main (String[] args) {
      int i = 2;
      while (i <= 200){
      System.out.println(i);
      i= i+2;
      }
   }
}


public class symbol {
    public static void main(String[] args) {
        int N=1;
         
         while (N <= 32) {
         N = 2*N;
         System.out.println(N);
         
        }
    }
}


public class square {
   public static void main (String[] args) {
      for (int i = 1; i<=12; i++){
         System.out.print("*");
         for (int j = 1; j<=5; j++){
            System.out.println("*     *");
         }
      }
   }
} 


public class nestedLoop{
   public static void main (String[] args) {
      for (int i = 1; i<=5; i++){
         for (int j = 4; j>=i; j--){
            System.out.print(8);
                 
         }
         System.out.println(i);
      }
   }
}


public class indefiniteloops{
public static void main (String[] args) {
      int i = 2;
      while (i <= 200){
      System.out.println(i);
      i= i+2;
      }
   }
}


import java.util.*;
public class Randoms {
public static void main (String[] args) {
   
   int die1;
   int die2;
   int sum;
   int tries;
   die1 = 0;
   die2 = 0;
   sum = 0;
   tries = 0;
   
          while(sum != 7){
                  
                  die1 = (int)(Math.random()*6)+1;
                  die2 = (int)(Math.random()*6)+1;
                  sum = (die1 + die2);
                  tries++;
                  System.out.println("your rolled a " + sum);
                  
          }
   System.out.println("You rolled " + tries +" times");
   }
}
