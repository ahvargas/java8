####Stream<T> filter(Predicate<? super T> predicate)

filter es una operacion intermedia. Obtine un stream que contiene
los elementos del stream que cumplen el predicado.
<!-- .element: class="fragment" -->

Esta es la interfaz del predicado.
<!-- .element: class="fragment" -->


```java
	public interface Predicate<T> {
        boolean test(T t);
    }
```
<!-- .element: class="fragment" -->


```java
	 fruitsStream
	 .filter( fruit -> fruit.contains("p"))
	 .forEach(System.out::println);
```
<!-- .element: class="fragment" -->
