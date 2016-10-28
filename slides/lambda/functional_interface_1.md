##¿Pero cual es el tipo de los lambdas? 

Se puede aplicar para mas tipos : <!-- .element: class="fragment" --> 

```java
	interface IntBinaryOperator {
        int apply(int left, int right);
    }

    interface LongBinaryOperator {
        long apply(long left, long right);
    }

```
<!-- .element: class="fragment" --> 

```java
	IntBinaryOperator withInt = (x, y) -> x + y;
    LongBinaryOperator withLong = (x, y) -> x + y;

    withInt.apply(1,1); //2
    withLong.apply(1,1); //2L
```
<!-- .element: class="fragment" --> 