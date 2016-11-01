####Stream<T> sorted(Comparator<? super T> comparator);

sorted es una operacion intermedia. Regresa un stream con los elementos
ordenados acorde al comparator.


<!-- .element: class="fragment" -->

Esta es la interfaz de Function.
<!-- .element: class="fragment" -->

```java
	@FunctionalInterface
    public interface Comparator<T> {
     * @param o1 the first object to be compared.
     * @param o2 the second object to be compared.
     * @return a negative integer, zero, or a positive integer as the
     *         first argument is less than, equal to, or greater than the
     *         second.
    int compare(T o1, T o2);
    }
```
<!-- .element: class="fragment" -->


```java
	 fruitsStream
        .sorted( (a,b) -> -1 * a.compareTo(b))
        .forEach(System.out::println);
```
<!-- .element: class="fragment" -->

```java
	 fruitsStream
         .sorted(Collections.reverseOrder())
         .forEach(System.out::println);
```
<!-- .element: class="fragment" -->

```java
	 fruitsStream
        .sorted()
        .forEach(System.out::println);
```
<!-- .element: class="fragment" -->


