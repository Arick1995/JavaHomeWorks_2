````Java
package searchstring;

import java.util.Scanner;

public class SearchString {

    public static void main(String[] args) {
         Scanner input = new Scanner(System.in);
         int a[]=new int[26];
         String b = input.nextLine();
         
         b.toLowerCase();
         
         for(int i = 0;i<b.length();i++){
             if(b.charAt(i)>='a' && b.charAt(i)<='z'){
                 a[b.charAt(i)-'a']++;
             }
         }
         
         System.out.println("a b c d e f g h i j k l m n o p q r s t u v w x y z");
         for(int i = 0;i<26;i++){
             System.out.print(a[i]);
             if(i<25)
                 System.out.print(" ");
             else
                 System.out.println();
         }
    }
    
}
