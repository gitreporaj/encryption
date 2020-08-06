# encryption
import java.io.*;
import java.util.*;
import java.text.*;
import java.math.*;
import java.util.regex.*;

public class Solution {

    public static String s;
    public static void main(String[] args) {
        Scanner input = new Scanner(System.in);
        s = input.next();
        int columnLen = (int) Math.ceil(Math.sqrt(s.length()));

        for(int i = 0; i < columnLen; i++)
        {    
            int j = i;
            while( j < s.length())
            {
                System.out.print(s.charAt(j));
                j+=columnLen;
            }
            if (i<columnLen-1) System.out.print(" ");
            else System.out.println();
        }
    }
}
