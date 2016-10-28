##¿Pero cual es el tipo de los lambdas? 



Una expresion lambda es una instancia de una interfaz funcional. <!-- .element: class="fragment" -->  

La expresion lambda en si no contiene información acerca del tipo que esta implementando, esta información es inferida por el contexto. Por ejemplo : <!-- .element: class="fragment" --> 

```java
interface IntBinaryOperator {
    int applyAsInt(int left, int right);
}

IntBinaryOperator operation = (x, y) -> x + y;

```
<!-- .element: class="fragment" --> 


