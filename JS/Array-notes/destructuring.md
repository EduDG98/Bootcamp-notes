# Destructuraci贸n 馃П

**脥NDICE**

1. [_Spread Operator_](#spread)
   1. [Funciones](#funciones)
   2. [_Arrays_](#arrays)
      1. [Asignaci贸n de variables](#asig)
   3. [Objetos](#obj)
2. [Cambio de estructura](#cambio)

# Destructuraci贸n

- Romper la estructura del array para asignar cada valor a las variables.
- La estrucutra se rompe a帽adiendo el _spread operator_.

# _Spread Operator_ (...) <a name='spread'></a>

- Sintanxis extendida.
- Sirve para referirise a 0, 1 o varios elementos en una funci贸n, _array_ u objecto.
- Lo que hace es romper la estructura que almacena la informaci贸n.

## Funciones:<a name='funciones'></a>

- <u>Ejemplo:</u>

  ```js
  const sum = (num1, num2, num3) => num1 + num2 + num3;

  const arrayOfNum = [2, 4, 6];
  console.log(sum(...arrayOfNum)); // 20
  ```

## _Arrays_:<a name='arrays'></a>

- Con el _spread operator_ se rompe la estructura y la a帽ade dentro del _array_ en la posici贸n deseada.
- <u>Ejemplo:</u>

  ```js
  	const mammals = ['dog', 'cat'. 'horse'];

  	cons animals = [...mammals, 'turtle', 'fox']; // ['dog', 'cat'. 'horse', 'turtle', 'fox']
  ```

### Asignaci贸n de variables:<a name='asig'></a>

- <u>Ejemplo:</u>
  ```js
  const [var1, var2, var3] = ["A", "B", 5];
  // var1 = 'A'
  // var2 = 'B'
  // var3 = 5
  ```
- Aplicando _spread operator_:
  ```js
  const [var1, ...var2] = ["A", "B", 5];
  // var1 = 'A'
  // var2 = ['B', 5]
  ```

## Objetos:<a name='obj'></a>

- Funciona igual que en los _arrays_.
- <u>Ejemplo:</u>

  ```js
  const isMammal = {
    dog: true,
    dolphin: true,
  };

  const hasEggs = {
    turtle: true,
    bird: true,
  };

  const animals = { ...isMammal, ...hasEggs }; // 	{dog: true, dolphin: true, turtle: true, bird: true}
  ```

> [!Recuerda]
> La mejor y forma recomendada para copiar _arrays_ y objectos es con _spread operator_.

# Cambio de estructura<a name='cambio'></a>

- Despu茅s de usar _spread operator_ para romper la estructura.
- Se puede poner en otra, lo que sirve para cambiar de una estructura a otra.

  - Como de objeto a _array_ o al rev茅s.

    - <u>Ejemplo:</u>

      ```js
      const isMammal = {
        dog: true,
        dolphin: true,
      };

      const arrayOfAnimals = [...isMammal]; // 	{dog, true, dolphin, true]
      ```
