###Métodos default

Se puede volver a hacer abstracto un metodo volviendo a definirlo en
otra interfaz. <!-- .element: class="fragment" -->

```java
interface Animal {
    default String talk(final String sentence) {
        return "Animal says: " + sentence;
    }
    default String walk() {
        return "Walking like a pro";
    }
}

interface Fish {
    String walk();
}

```
<!-- .element: class="fragment" -->

```java
final class Goldfish implements Fish {} // Esto compila?
```
<!-- .element: class="fragment" -->
No compila (Goldfish is not abstract and does not override abstract
method walk() in Fish).
<!-- .element: class="fragment" -->

```java
class Hake implements Fish {
    @Override
    public String walk() {
        return "Fish don't walk";
    }
}
```
<!-- .element: class="fragment" -->
