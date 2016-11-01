####<R> Stream<R> map(Function<? super T, ? extends R> mapper);

Como se ve el tipo de salida no tiene que ser el mismo que entra. Lo
que permite transformar de un tipo a otro.
<!-- .element: class="fragment" -->


```java
	@Value
    class Fruit {
        private final String name;
    }

    fruitsStream
        .map(Fruit::new)
        .forEach(System.out::println);
```
<!-- .element: class="fragment" -->


