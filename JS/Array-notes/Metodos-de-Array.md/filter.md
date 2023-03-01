# filter()

- Ejecuta una _callback_.
- Delvuelve los elementos que cumplen la condición de la _callback_.
- <u>Ejemplo:</u>
  ```js
  const myArray = ["Manuel", "Pepe", "Lorena"];
  myArray.filter((name) => {
    return name.length == 4;
  });
  // Pepe
  ```
