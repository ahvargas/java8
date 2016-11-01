####boolean anyMatch(Predicate<? super T> predicate);

anyMatch es una operacion de corto circuito. Regresa verdadero si algun
elemento del stream cumple el predicado




```java
	  fruitsStream
         .anyMatch( fruit -> fruit.startsWith("p")); //true
```
<!-- .element: class="fragment" -->

```java
	  fruitsStream
          .anyMatch(contains("p")); //true
```
<!-- .element: class="fragment" -->



