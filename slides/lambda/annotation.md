## Definición formal


Una interfaz funcional tiene exactamente un método abstracto. 

Como las interfaces ahora pueden tener una implementación por defecto, estos métodos no son abstractos 


En Java 8 un interfaz que tiene declarado un único método abstracto se considera un interfaz funcional y esta representado por un “Functional Descriptor”. Cuando hablamos de “Functional Descriptor” de un interfaz nos referimos a la firma del método abstracto, que está compuesta por sus parámetros, el tipo de los parámetros, el tipo que devuelve el método y las excepciones que lanza:


Vemos que el interfaz tiene declarados dos métodos abstractos (además de varios métodos estáticos y default). Uno de estos es el método compare y otro es el método equals, que sobrescribe el método de la clase Object. Éste interfaz no se ajustaría a la anterior definición de interfaz funcional al tener dos métodos abstractos, pero en la definición de interfaz funcional se indica que en un interfaz pueden existir múltiples métodos abstractos siempre que todos menos uno sobrescriban un método público de la clase Object.

Ahora se pueden añadir métodos default o static a los interfaces pero estos métodos no son abstractos, de modo que un interfaz funcional podrá tener tantos métodos de este tipo como se desee.

Además, se ha creado una nueva anotación, @FunctionalInterface, para indicar la intención de ser un interfaz funcional, produciendo un error de compilación si el interfaz no cumple las características de un interfaz funcional. Al igual que @Override, esta notación no es obligatoria pero es recomendable su uso para mejorar la legibilidad.

Los interfaces funcionales están muy relacionados con las expresiones lambdas. Cuando ejecutamos una expresión lambda esta es convertida a un interfaz funcional, donde el cuerpo de la expresión lambda es la implementación del método abstracto. En un siguiente articulo intentaré explicar mejor las expresiones lambda para que se entienda mejora la relación que tienen con los interfaces funcionales.


```java
	(final int x, final int y) -> { return x + y; };
``` 


a functional interface has exactly one abstract method. Since default methods have an implementation, they are not abstract. If an interface declares an abstract method overriding one of the public methods of java.lang.Object, that also does not count toward the interface's abstract method count since any implementation of the interface will have an implementation from java.lang.Object or elsewhere