##Method references

Se pueden usar expresiones lambda para crear metodos anonimos. Pero
a veces la expresion lambda no hace nada mas que llamar a un metodo
existente. Las refencias a los metodos permiten ahorrarnos la expresion
lambda.

<!-- .element: class="fragment" -->


```java
	@FunctionalInterface
    interface Person {
        String talk();
    }
    class Coder  {
        String code() {
            return "Hello world!";
        }
    }
    class Conference {
        String lecture(Person person){
            return person.talk();
        }
    }
    val c = new Conference();
    val coder = new Coder();

    c.lecture(() -> coder.code());
```
<!-- .element: class="fragment" -->


```java
	c.lecture(coder::code);
```
<!-- .element: class="fragment" -->
