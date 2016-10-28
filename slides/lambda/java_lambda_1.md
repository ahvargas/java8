###Sintaxis de expresiones lambda en java

Si solo se pone una expresión se puede eliminar las llaves y el return: <!-- .element: class="fragment" --> 
```java
	(final int x, final int y) -> x + y;
``` 
<!-- .element: class="fragment" --> 

También se puede eliminar los tipos de los parámetros de entrada: <!-- .element: class="fragment" --> 
```java
	(x, y) -> x + y;
``` 
<!-- .element: class="fragment" --> 