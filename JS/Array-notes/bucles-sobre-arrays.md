# Bucles sobre Arrays ➰➰➰

**ÍNDICE**

1. [`for in`](#in)
2. [`for of`](#of)
3. [`forEach()`](#each)

# _for in_<a name='in'></a>

- Recorre las posiciones.
- <u>Ejemplo:</u>
  ```js
  for (let i in array){
  	const elemento = array[i];
  	console.log(`El elemento es ${elemento} y la posicion ${i});
  }
  ```

# _for of_<a name='of'></a>

- Recorrere los elementos.
- <u>Ejemplo:</u>
  ```js
  for (let elmento of array){
  	console.log(`El elemento es ${elemento});
  }
  ```

# _forEach()_<a name='each'></a>

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
  - _elemento_ del array
  - _posición_ del array
  - al _array_
- <u>Ejemplo:</u>
  ```js
  const myArray = ["A", "B", "C"];
  myArray.forEach(function (element, index, array) {
    console.log(`El elemento ${element} está en la posicion ${index}`);
  });
  ```
