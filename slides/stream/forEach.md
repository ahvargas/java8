###void forEach(Consumer<? super T> action)

forEach metodo es terminal.
<!-- .element: class="fragment" -->

Itera sobre los elementos de un stream y ejectuta una operacion.
La expresion a ejecutar es de tipo Consumer.
<!-- .element: class="fragment" -->


```java
	public interface Consumer<T> {
        void accept(T t);
    }
```
<!-- .element: class="fragment" -->

```java
	fruitsStream.forEach(new Consumer<String>() {
        @Override
        public void accept(String fruit) {
            System.out.println(fruit);
        }
    });
```
<!-- .element: class="fragment" -->

```java
	fruitsStream.forEach( fruit -> System.out.println(fruit));
```
<!-- .element: class="fragment" -->


```java
	fruitsStream.forEach(System.out::println);
```
<!-- .element: class="fragment" -->
