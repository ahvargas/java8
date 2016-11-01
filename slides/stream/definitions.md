##Streams

Secuencia de elementos (Stream) : Un stream es una interfaz para
acceder de manera secuencial a un conjunto de valores.
<!-- .element: class="fragment" -->

Los stream no necesariamiante tienen que almacenar los elementos
, se generan bajo demanda.
<!-- .element: class="fragment" -->

```java
	IntSupplier infinite = new IntSupplier() {
        private int value = 0;
        @Override
        public int getAsInt() {
            return value++;
        }
    };
    final IntStream infinite = IntStream.generate(infinite);
```
<!-- .element: class="fragment" -->


```java
    Stream<Double> randomNumbers = Stream.generate(Math::random);
```
<!-- .element: class="fragment" -->

