####<R> Stream<R> map(Function<? super T, ? extends R> mapper);

map es una operacion intermedia. Obtine un stream que contiene
los elementos del stream aplicando la funcion a cada elemento.

<!-- .element: class="fragment" -->

Esta es la interfaz de Function.
<!-- .element: class="fragment" -->

```java
	public interface Function<T, R> {
        R apply(T t);
    }
```
<!-- .element: class="fragment" -->


```java
	fruitsStream
        .map(String::toUpperCase)
        .forEach(System.out::println);
```
<!-- .element: class="fragment" -->


