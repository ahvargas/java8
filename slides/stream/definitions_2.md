##Streams

Funciones de agregación: Los stream incorporan funciones para ser
utilizados como : filter, map , reduce, find.

<!-- .element: class="fragment" -->

Estas operaciones tienen una caracteristica importante:

<!-- .element: class="fragment" -->

Canalización (Pipelining) : Las operaciones no terminales ,
 regresan otro stream. Como consecuencia las operaciones se
pueden enlazar como si se tratara de una tuberia.

<!-- .element: class="fragment" -->


```java
	infinite
	    .skip(5)
	    .filter(x -> x%2 == 0)
	    .findAny()
	    .getAsInt(); // 6
```
<!-- .element: class="fragment" -->
