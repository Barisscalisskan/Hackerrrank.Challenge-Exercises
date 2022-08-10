import java.util.*;
import java.io.*;


public class Solution {
    
public static void main(String[] args) {


Scanner bar = new Scanner(System.in);

int t = bar.nextInt();

for (int i = 0; i < t; i++) {

try 
{

long x = bar.nextLong();

System.out.println(x + "can be fitted in:");

if (x >= -128 && x <= 127) System.out.println("* byte");

if (x >= -32768 && x <= 32767) System.out.println("* short");

if (x >= Math.pow(-2,31) && x <= Math.pow(2,31) - 1) System.out.println("* int");

if (x >= Math.pow(-2, 63) && x<= Math.pow(2,63) - 1) System.out.println("* long");


} catch (Exception e) {

System.out.println(bar.next() + " can't be fitted anywhere. ");
            
}

}


}


}

