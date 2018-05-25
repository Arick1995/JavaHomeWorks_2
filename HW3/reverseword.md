````Java
package reverseword;

import java.util.Scanner;

public class ReverseWord {

    public static void main(String[] args) {
        Scanner input = new Scanner(System.in);
        String sc;
        
        System.out.println("Input a sentence : ");
        sc = input.nextLine();
        
        String[] tokens = sc.split(" ");
        String rs = "";
        for(int i = tokens.length-1;i>=0;i--){
            rs+=tokens[i]+" ";
        }
        System.out.printf("Reversed : \n");
        System.out.printf(rs);
    }
    
}
