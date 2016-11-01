####<R, A> R collect(Collector<? super T, A, R> collector);

collect es una operacion terminal. Recolecta los elementos del stream
en una colección.
<!-- .element: class="fragment" -->


Esta es la interfaz de Collector.
<!-- .element: class="fragment" -->



```java
	 interface Collector<T,A,R> {
         Supplier<A>          supplier()
         BiConsumer<A,T>      acumulator()
         BinaryOperator<A>    combiner()
         Function<A,R>        finisher()
         Set<Characteristics> characteristics()
     }
```
<!-- .element: class="fragment" -->

La interfaz es un poco mas complicada que las demas y queda fuera del
ámbito de esta charla. Ver [aqui](http://www.nurkiewicz.com/2014/07/introduction-to-writing-custom.html)

<!-- .element: class="fragment" -->

```java
	List<String> sortedFruits = fruitsStream
        .sorted()
        .collect(Collectors.toList());
```
<!-- .element: class="fragment" -->



