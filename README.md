import java.util.Scanner;
public class Decimal_BinaryString_PartC
 {
    public static void main(String[]args) 
    {  Scanner input=new Scanner(System.in);

        System.out.print("Enter an integer: ");
        int num=input.nextInt();

        String binary=toBinaryString(num);
        System.out.println("Binary: " + binary);
    }

public static String toBinaryString(int num) 
   {
        String binary = "";

      while(num>0) 
        {
            binary=(num % 2) + binary;
            num /= 2;
        }

        return binary;
   }
 }
