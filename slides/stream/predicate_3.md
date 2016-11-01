##Predicate

Creando una funcion que devuelve interfaces funcionales:
<!-- .element: class="fragment" -->


```java
	Predicate<String> contains(final String s) {
        return fruit -> fruit.contains(s);
    }
```
<!-- .element: class="fragment" -->

```java
	Predicate<String> p = contains("p");
    Predicate<String> a = contains("a");
    fruitsStream.filter(p.and(a)).forEach(System.out::println);
```
<!-- .element: class="fragment" -->


```java
	fruitsStream
        .filter(contains("p").and(contains("a")))
        .forEach(System.out::println);
```
<!-- .element: class="fragment" -->
