# every() & some()

# `every()`

- Ejecuta una _callback_.
- Si **todos** los elementos del array cumple la condición de la _callback_ devuelve algo.
- <u>Ejemplo:</u>
  ```js
  const myArray = ["A", "B", "C"];
  myArray.every((element) => {
    if (element.length == 1) {
      return true;
    }
  });
  // true
  ```

# `some()`

- Ejecuta una _callback_.
- Si **alguno** de los elementos del array cumple la condición de la _callback_ devuelve algo.
- <u>Ejemplo:</u>
  ```js
  const myArray = ["A", "B", "CC"];
  myArray.some((element) => {
    if (element.length == 2) {
      return true;
    }
  });
  // true
  ```
