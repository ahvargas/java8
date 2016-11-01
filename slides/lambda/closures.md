##Clousure

Un clousure(cierre) es una función que utiliza variables definidas
fuera del alcance de la función.
<!-- .element: class="fragment" -->

```java
	interface Adder {
        int add(int x);
    }

    static Adder makeAdder(final int n) {
        return (x) -> x + n;
    }

    makeAdder(3).add(5); //8
```
<!-- .element: class="fragment" -->

La función (x) -> x + n; es un clousure por que utiliza la variable n
que esta definida fuera de su alcance.
<!-- .element: class="fragment" -->
