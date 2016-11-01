# Cálculo lambda

Toda función que requiere dos argumentos, como por ejemplo la función
suma, puede ser reescrita como una función que acepta un único
argumento, pero que devuelve otra función, la cual a su vez acepta un
único argumento. Por ejemplo, x,y → x + y puede ser reescrita como
x → (y → x + y). <!-- .element: class="fragment" -->

[Esta transformación se conoce como currificación](https://en.wikipedia.org/wiki/Currying) <!-- .element: class="fragment" -->
