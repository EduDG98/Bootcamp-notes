# M茅todos de Array 馃捈

- `push()` --> a帽ade un elemento por el final del array.
- `pop()` --> elimina el 煤ltimo elemento y lo devuelve.
- `shift()` --> elimina el primer elemento y lo devuelve.
- `unshift()` --> agrega uno o varios elementos al principio del array.

- `concat()` --> unir dos en un mismo _array_.
- `flat()` --> concaneta los subarrays dentro de un _array_ (bajanado un nivel)
- `sort()` --> ordena un array seg煤n su _ascii_.
- `join()` --> junta una los elementos del array con un elemento separador especificado y todo eso lo convierte a una 煤nica _string_.
- `reverse()` --> invierte el orden de _array_.

- `indexOf(elemento)` --> dado un elmento del _array_ devuelve la posici贸n del primero que haya.
- `lastIndexOf(elemento)` --> dado un elmento del _array_ devuelve la **posici贸n del 煤ltimo** que haya.

- `forEach()` --> ejecuta una _callback(element, index, array)_ en cada elemento del array. **No devuelve nada**.
- `map()` --> recorre el _array_ elemento por elemento.
- `every()` --> devuelve algo si **todos** los elementos cumple la condici贸n de la _callback_.
- `some()` --> si **alguno** de los elementos del _array_ cumple la condici贸n devuelve algo.
- `find()` --> devuelve el **primer** elemento del _array_ que cumpla la condici贸n del _array_.
- `includes()` --> devuelve **_true/false_** si el _array_ tiene el _element_.

- `reduce()` --> devuelve un valor 煤nico al reducir los elementos del _array_-
- `filter()` --> devuelve los elementos que cumplen la condici贸n en el _callback_.

- `slice()` --> devuelve una **copia** de una porci贸n del array en un nuevo array.
  - `slice(n1, n2)`
- `splice()` --> agrega o elimina elementos del array **original** en una posicion especificada.

  - `splice(n1, n2)` --> elimina lo que haya entre las posiciones _n1_ y _n2_
  - `splice(n1, n2, char)` --> elimina lo que haya entre las posiciones _n1_ y _n2_ y coloca el _char_.
    > Los n潞 corresponde a los espacios, emepezando por 0.

- `at(n)` --> para buscar el elemento en la posici贸n _n_. Es como `arrayName[n]`
