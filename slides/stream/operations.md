##Api

Ahora hablaremos un poco del api. Los streams tienen 3 tipos de
operaciones:<!-- .element: class="fragment" -->

- Intermedias. Regresan un stream con el cual podemos seguir trabajando.
<!-- .element: class="fragment" -->
- Terminales. Devuelven un tipo de dato diferente al stream. Una vez
que se invoca a una operacion terminal el stream queda cerrado y no
se puede trabajar mas con el.
<!-- .element: class="fragment" -->
(java.lang.IllegalStateException: stream has already been operated
 upon or closed)
<!-- .element: class="fragment" -->
- Corto circuito.
<!-- .element: class="fragment" -->

