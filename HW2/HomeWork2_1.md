````java
package homework2;

import javax.swing.JOptionPane;

public class HomeWork2_1 {
    
    public static void main(String[] args){
        
        String num1 = JOptionPane.showInputDialog("First number ?");
        String num2 = JOptionPane.showInputDialog("Second number ?");
        
        int sum = Integer.parseInt(num1)+Integer.parseInt(num2);
        
        String message = String.format("%s + %s = %d",num1,num2,sum);
        
        JOptionPane.showMessageDialog(null,message);
        
    }
}
