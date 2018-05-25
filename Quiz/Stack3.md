```java
/*
 * To change this license header, choose License Headers in Project Properties.
 * To change this template file, choose Tools | Templates
 * and open the template in the editor.
 */
package stacktest_3;
import java.util.ArrayList;



/**
 *
 * @author aa
 */
public class Stack3<T> {
    private ArrayList< T > elements; // ArrayList stores stack elements

   // no-argument constructor creates a stack of the default size
   public Stack3()
   {
      this( 10 ); // default stack size
   } // end no-argument Stack constructor
   
   // constructor creates a stack of the specified number of elements
   public Stack3( int capacity )
   {
      int initCapacity = capacity > 0 ? capacity : 10; // validate
      elements = new ArrayList< T >( initCapacity ); // create ArrayList
   } // end one-argument Stack constructor

   // push element onto stack
   public void push( T pushValue )
   {
      elements.add( pushValue ); // place pushValue on Stack
   } // end method push

   // return the top element if not empty; else throw EmptyStackException
   public T pop()
   {
      if ( elements.isEmpty() ) // if stack is empty
        System.exit(1);
    
      // remove and return top element of Stack
      return elements.remove( elements.size() - 1 ); 

   }
}
