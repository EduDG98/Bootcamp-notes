# find() & findIndex()

# `find()` & `findLast()`

- Ejecuta una _callback_.
- Devuelve el primer elmento que cumpla la condicción de la _callback_.
- <u>Ejemplo:</u>
  ```js
  const students = [
    { name: Manuel, age: 20 },
    { name: Pepe, age: 15 },
    { name: Lorena, age: 30 },
  ];
  students.find((studentItem) => {
    return studentItem.age > 15;
  });
  // {name: Manuel, age:20}
  ```

# `findIndex()` & `findLastIndex()`

- Ejecuta una _callback_.
- Devuelve la primera posición del elmento que cumpla la condicción de la _callback_.
- <u>Ejemplo:</u>
  ```js
  const students = [
    { name: Manuel, age: 20 },
    { name: Pepe, age: 15 },
    { name: Lorena, age: 30 },
  ];
  students.find((studentItem) => {
    return studentItem.age > 15;
  });
  // {name: Manuel, age:20}
  ```
