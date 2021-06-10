## Calc
```
public class Calc {
    static public int add(int a, int b) {
        return a + b;
    }

    static public int sub(int a, int b) {
        return a - b;
    }

    static public int multi(int a, int b) {
        return a * b;
    }

    static public int div(int a, int b) {
        return(float) a / b;
    }
}
```

## CalcTest
```
import org.junit.Test;
import static org.junit.Assert.*;
import java.util.*;

public class CalcTest {
  int a;
  int b;
  float result;
  
  public CalcTest(int a, int b, float result) {
    a = 16;
    b = 4;
    this.result = result;
   }
  
  @Test
  public void testAdd() {
        assertEquals(Calc.add(a, b), 20);
    }
    
  @Test
  public void testMinus() {
        assertEquals(Calc.sub(a, b), 12);
    }

  @Test
  public void testMultiply() {
        assertEquals(Calc.multi(a, b), 64);
    }

  @Test
  public void testDivide() {
        assertEquals(Calc.div(a, b), 4, 0.25);
    }
}
```
