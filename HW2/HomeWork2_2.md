````java
package homework2;

import java.awt.Graphics;
import javax.swing.JPanel;

public class HomeWork2_2 extends JPanel {
    private int ts;
    
    public HomeWork2_2(int te){
        ts = te;
    }
    public void paintComponent(Graphics g){
        super.paintComponent(g);
        int radius = 10;
        
        for(int i= 0;i<=ts;i++){
            g.drawOval(145-(radius*2+i*10)/2,135-(radius*2+i*10)/2, radius+i*10, radius+i*10);
        }
    }
}
