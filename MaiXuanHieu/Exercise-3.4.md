'''
import junit.framework.*;

import org.junit.Test;

import static org.junit.Assert.assertEquals;

public class BoundedQueueTest {
  BoundedQueue instance = new BoundedQueue(3);
  
  public void enQueueTest() {
      for(int i = 1; i < 4; i++) {
          instance.enQueue(i);
          }
      assertEquals(instance.toString(), "[1, 2, 3]");
     }    
  
  public void deQueueTest {
      for (int i = 1; i < 4; i++){
            q.enQueue(i);
            }
        assertEquals(q.deQueue(), 1);
        assertEquals(q.deQueue(), 2);
        assertEquals(q.deQueue(), 3);
        
  public void isEmptyTest {
      assertEquals(instance.isEmpty(), true);
      }
      
  public void isFullTest {
      assertEquals(instance.isFull(), true);
      }
      
  public void toStringTest {  
      }
}
'''
