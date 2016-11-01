###Sintaxis de expresiones lambda en java

Una lista separada por comas de parámetros formales entre paréntesis.  <!-- .element: class="fragment" --> 

Una flecha (arrow token)<!-- .element: class="fragment" -->   ``` -> ``` <!-- .element: class="fragment" --> 


Un cuerpo compuesto: Por una expresion  <!-- .element: class="fragment" --> 


```java
	(final int x, final int y) -> { return x + y; };
``` 
<!-- .element: class="fragment" --> 

O un bloque (conjunto de expresiones)
<!-- .element: class="fragment" --> 

```java
	(final int x, final int y) -> {
        int result = x + y;
        return result;
    };
``` 
<!-- .element: class="fragment" --> 

