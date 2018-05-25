````java
/*
 * To change this license header, choose License Headers in Project Properties.
 * To change this template file, choose Tools | Templates
 * and open the template in the editor.
 */
package stacktest_3;

/**
 *
 * @author aa
 */
public class StackTest_3 {

    /**
     * @param args the command line arguments
     */
    public static void main(String[] args) {
        Stack3< Integer > integerStack = new Stack3< Integer >(); 
        Stack3< Double > doubleStack = new Stack3< Double >(); 
        String[] a = {"push", "12", "push", "33", "pop", "pop"};
        String[] b = {"push", "1.2", "push", "3.3", "pop", "pop", "push", "6.3", "pop"};
        Integer v;  
        Double w;
        
        int int_value;
        double double_value;
        int i = 0;
        while ( i < a.length){  
            if (a[i].equals("push")){ 
                i++;
                int_value = Integer.parseInt(a[i]);
                v = new Integer(int_value);
                testPush( integerStack, v);
            }
        else
           testPop( integerStack ); // pop from integerStack
        i++;	
        }
        i = 0;
        while ( i < b.length){  
            if (b[i].equals("push")){ 
                i++;
            double_value = Double.parseDouble(b[i]);
            w = new Double(double_value);
            testPush( doubleStack, w);
        }
        else
           testPop( doubleStack ); // pop from integerStack
        i++;	
        }
    } // end main

   private static <T> void testPush( 
      Stack3<T> stack,  T value )
   {
      System.out.println( "\nPushing a value onto Stack" );
      System.out.printf( "%s ", value );
      stack.push( value ); // push onto integerStack
   } // end method testPushInteger

   private static <T> void testPop( Stack3< T> stack )
   {
         System.out.println( "\nPopping a value from Stack" );
         T popValue;
    
         popValue = stack.pop(); // pop from Stack
         System.out.printf( "%s ", popValue );
   } // end method testPop


    }
    
