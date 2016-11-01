##Clousure

En java los clousures actuan por valor, y las variables que defininen
deben de ser finales o ser efectivamente finales. Es decir que no
cambian de valor.
<!-- .element: class="fragment" -->

```java
	interface Adder {
        int add(int x);
    }

    static Adder wrongAdder(int n) {
            return (x) ->  {
                n = n +1 ;
                return x + n;
            }
        }
```
<!-- .element: class="fragment" -->


El mensaje de error es : local variables referenced from a lambda
expression must be final or effectively final.
<!-- .element: class="fragment" -->
