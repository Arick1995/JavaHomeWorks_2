````java
package homework2;

import javax.swing.JFrame;
import javax.swing.JOptionPane;

public class HomeWork2_2_test {
    public static void main(String[] args){
        String input = JOptionPane.showInputDialog("How many times to draw the circle ?");
        
        int time = Integer.parseInt(input);
        HomeWork2_2 panel = new HomeWork2_2(time);
        JFrame application = new JFrame();
        
        application.setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
        application.add(panel);
        application.setSize(300,300);
        application.setVisible(true);
    }
    
}
