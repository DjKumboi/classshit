# class



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




import java.util.*;
import java.io.*;
public class Cha{
public static void main(String[]args) throws FileNotFoundException {
//Scanner input = new Scanner(System.in);
Scanner input = new Scanner(new File("test.txt"));
String word = "";
int sum = 0;
int count = 0;
while (input.hasNextInt()){
sum = sum + input.nextInt();
count++;
}
System.out.println("Average temperature: " + (sum/count));
input.close();
}
}




import java.util.*;
import java.io.*;
public class Cha{
public static void main(String[]args) throws FileNotFoundException {
Scanner input = new Scanner(new File("test.txt"));
String word = "";
int sum = 0;
int count = 0;
while (input.hasDouble()){
System.out.println(input.nextDouble());
}
//System.out.println("Change in temperature:" + (sum/count));
input.close();
}
}




import java.util.*;
import java.io.*;
public class hoursworked{
public static void main(String[]args) throws FileNotFoundException {
Scanner jobs = new Scanner(new File("hours.txt"));
   while(jobs.hasNextLine()){
      String line = jobs.nextLine();
      Scanner lineScan = new Scanner(line);
      int id = (lineScan.nextInt());
      String name = (lineScan.next());
      double totalHours = 0.0;
      int days = 0;
         while (lineScan.hasNextDouble()){
            totalHours += lineScan.nextDouble();
            days++;
      }
      System.out.println(name + " (ID%" + id + ") worked " + totalHours + "hours (" + (totalHours/days) + "hours/day)");
   }
}
}
      


Version 2 printstream

import java.util.*;
import java.io.*;
public class hoursworked{
public static void main(String[]args) throws IOException {
PrintStream outfile = new PrintStream( new File ("hours_out.txt"));
Scanner jobs = new Scanner(new File("hours.txt"));
   while(jobs.hasNextLine()){
      String line = jobs.nextLine();
      Scanner lineScan = new Scanner(line);
      int id = (lineScan.nextInt());
      String name = (lineScan.next());
      double totalHours = 0.0;
      int days = 0;
         while (lineScan.hasNextDouble()){
            totalHours += lineScan.nextDouble();
            days++;
      }
      outfile.println(name + " (ID%" + id + ") worked " + totalHours + "hours (" + (totalHours/days) + "hours/day)");
   }
}
}



PrintStream

import java.util.*
import java.io.*
public class Stream {
   public static void main(String[]args) throws IOException{
      PrintStream outfile = new PrintStream( new File ("Streamtest.txt"));
         outfile.println("hello");
         outfile.println("Steven Senegal");
         outfile.println("action is coming");
         outfile.println("hello");
         outfile.println("hello");
         outfile.println("hello");
         outfile.println("hello");
         outfile.println("hello");
         outfile.println("hello");
         outfile.println("hello");
     
}
}


printf version
import java.util.*;
import java.io.*;
public class hoursworked{
public static void main(String[]args) throws IOException {
PrintStream outfile = new PrintStream( new File ("hours_out.txt"));
Scanner jobs = new Scanner(new File("hours.txt"));
   while(jobs.hasNextLine()){
      String line = jobs.nextLine();
      Scanner lineScan = new Scanner(line);
      int id = (lineScan.nextInt());
      String name = (lineScan.next());
      double totalHours = 0.0;
      int days = 0;
         while (lineScan.hasNextDouble()){
            totalHours += lineScan.nextDouble();
            days++;
      }
      outfile.printf(name + " (ID#" + id + ") worked " + totalHours + "hours (%.2f" , (totalHours/days)); 
      outfile.print("hours/day)");
      outfile.println();
   }
}
}
      
