##Streams

- Fuente: Los streams consumen datos de una fuente. Por ejemplo un lista,
un array , un socket, etc..

<!-- .element: class="fragment" -->

```java
	List<Integer> list = new ArrayList<>();
    for(int i = 0; i< 10; i++){
        list.add(i);
    }
    Stream<Integer> stream = list.stream();
```
<!-- .element: class="fragment" -->


```java
    Stream<Integer> stream = Stream.of(0,1,2,3,4,5,6,7,8,9);
```
<!-- .element: class="fragment" -->
