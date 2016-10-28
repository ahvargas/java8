##Métodos default

```java
interface Animal {
    default String talk(final String sentence) {
        return "Animal says: " + sentence;
    }
}
```
<!-- .element: class="fragment" --> 



```java
class Snake implements Animal {}


final Animal snake = new Snake();
snake.talk("what?"); // "Animal says: what?"
```
<!-- .element: class="fragment" --> 