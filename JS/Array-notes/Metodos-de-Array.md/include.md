# include

- Deuvelve un _boolean_ si el elemento está en el _array_.
- Hay dos parámetros en el _include()_
  - el valor para saber si está incluido
  - el índice del _array_ donde empieza
- <u>Ejemplo:</u>
  ```js
  const myArray = ['Manuel', 'Pepe', 'Lorena'];
  myArray.include(('Pepe')  // true
  ```

## Filtrar de en un array con otro

- <u>Ejemplo:</u>
  ```js
  const array1 = [1,2,3,4,5];
  const array2 = [2,4,6]
  array1.filter( item => array2.includes(item)  // [2,3]
  ```
