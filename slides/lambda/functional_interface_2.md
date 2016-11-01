##Generics

```java
	interface GenericOperator<T> {
        T apply(T left, T right);
    }

```
<!-- .element: class="fragment" -->

```java
	GenericOperator<String> withString = (x, y) -> x + y;
    withString.apply("Lam", "bda"); //Lambda
```
<!-- .element: class="fragment" -->

No se puede usar un interfaz funcional si el metodo de la interfaz
funcional tiene parametros de <!-- .element: class="fragment" -->  [tipo](http://docs.oracle.com/javase/specs/jls/se8/html/jls-15.html#jls-15.27.3) <!-- .element: class="fragment" -->

```java
    interface NoCompile {
        <T> T apply(T left, T right);
    }

    NoCompile bad = (String x, String y) -> x + y;

```
<!-- .element: class="fragment" -->
