# Array - Básico 🎹

1. [Crear un _array_](#crear)
2. [Modificar un _array_](#modificar)
3. [Propiedades de _arrays_](#prop)

# _Arrays_

- Es un objeto (una estructura de dato) y se puede almacenar una coleccion de valores de cualquier tipo de JS.

## Crear _un_ array:<a name='crear'></a>

- **Forma 1**:
  ```js
  const arrayName = ["value1", "value2", "value3"];
  ```
- **Forma 2**: llamando a la clase **_Array_**
  ```js
  const arrayName = new Array("value1", "value2", "value3");
  ```

## Modificar un _array_:<a name='modificar'></a>

- **Acceder** a un elemento del _array_:
  ```js
  const arrayName = ["value1", "value2", "value3"];
  const primerValor = arrayName[0];
  ```
- **Modificar** el elemento en el array:
  ```js
  const arrayName = ["value1", "value2", "value3"];
  const primerValor = 1; // [1, 'value2', 'value3']
  ```

## Propiedades de _arrays_:<a name='prop'></a>

- Las propiedades se diferencia visualemente de los métodos porque van sin paréntesis.
- Las propiedades más usada es:
  - `.length` --> devuelve la longitud del _array_.
