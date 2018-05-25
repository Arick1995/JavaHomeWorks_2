```java
package phonenumbertoken;

import java.util.Scanner;
import java.util.StringTokenizer;

public class PhoneNumberToken {

    public static void main(String[] args) {
        Scanner input = new Scanner(System.in);
        String PN;
        
        System.out.println("Input the Phone Number : ");
        PN = input.nextLine();
        
        String[] token = PN.split("\\(|\\)| |-");
        String ac = token[1];
        String num = token[3]+token[4];
        System.out.printf("Area Code = %s\nPhone Number = %s\n",ac,num);
    }
    
}
