##Predicate

Lo que nos permite hacer cosas como :
<!-- .element: class="fragment" -->


```java
	Predicate<String> p = fruit -> fruit.contains("p");
    Predicate<String> a = fruit -> fruit.contains("a");
    fruitsStream.filter(p.and(a)).forEach(System.out::println);
```
<!-- .element: class="fragment" -->

```java
	Predicate<String> p = fruit -> fruit.contains("p");
    Predicate<String> a = fruit -> fruit.contains("a");
    fruitsStream.filter(p.or(a)).forEach(System.out::println);
```
<!-- .element: class="fragment" -->


```java
	Predicate<String> p = fruit -> fruit.contains("p");
    fruitsStream.filter(p.negate()).forEach(System.out::println);
```
<!-- .element: class="fragment" -->
