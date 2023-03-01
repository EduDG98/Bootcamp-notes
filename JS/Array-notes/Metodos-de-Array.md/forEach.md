# forEach()

- Ejecuta una función _callback_ a cada elemento del array.
- Nunca devuelve nada.
- <u>Ejemplo:</u>
  ```js
  const myArray = ["A", "B", "C"];
  myArray.forEach(function () {
    console.log("Hey");
  });
  ```

## Callbak del forEach()

- En la función _callback_ se pueden pasar argumentos.
- Los primeros argumentos estan reservados para referirse:
  - elemento del array.
  - posición del array.
  - al array.
- <u>Ejemplo:</u>
  ```js
  const myArray = ["A", "B", "C"];
  myArray.forEach(function (element, index, array) {
    console.log(`El elemento ${element} está en la posicion ${index}`);
  });
  ```
