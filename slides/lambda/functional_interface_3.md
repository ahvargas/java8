
El tipo de los lambda

The type expected for the expression on the right-hand side of the assignment here is IntOperation. This is called the target type for the lambda expression. Clearly a lambda expression can be type-compatible with different functional interfaces, so it follows that the same lambda expression can have different target types in different contexts. For example, given an interface



Una interfaz funcional tiene exactamente un metodo abstracto. 


```java
	(final int x, final int y) -> { return x + y; };
``` 


a functional interface has exactly one abstract method. Since default methods have an implementation, they are not abstract. If an interface declares an abstract method overriding one of the public methods of java.lang.Object, that also does not count toward the interface's abstract method count since any implementation of the interface will have an implementation from java.lang.Object or elsewhere