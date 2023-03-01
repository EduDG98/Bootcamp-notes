# Objectos 🧩

**ÍNDICE**
1. [Estructura de un objecto](#estructura)
2. [Añadir una propiedad](#añadir)
3. [Acceder a una propiedad](#acceder)
4. [*Getter* & *Setter*](#getter)
5. [Bucles en los Objetos](#bucles)

# Estructura de un objeto:<a name='estructura'></a>
- Los objetos están formados por propiedades que tiene valores
- Y funciones que son métodos de los objetos (para cambiar las propiedades del objeto)
- <u>Ejemplo:</u>
	```js
		const objectName = {
			prop1: 'value1',  // Propiedad del objeto.
			prop2: 10,        // Otra propiedad del obj.
			sum = (num)       // Método del objeto.
		}
	```


# Añadir una propiedad<a name='añadir'></a>
## Si la propiedad existe:
- <u>Ejemplo:</u>
	```js
	const person = {
		name = 'Peter',
		age = 22
	};

	person.name = 'Jhon';
```
## Si la propiedad no existe:
- <u>Ejemplo:</u>
	```js
	const person = {}

	person.name = 'Jhon';
	person.sayHi = () => console.log('Hey');
```

# Acceder a una propiedad<a name='acceder'></a>
- Hay dos formas:
1. ``obj.prop1``
2. ``obj[prop1]``
	- Esta forma se usa cuando el nombre de la propiedad tiene un espacio entre las palabras.
	- O si el nombre de la propiedad es un número.


# Getter & Setter<a name='getter'></a>
- Son funciones especiales dentro de los objetos (en este caso)
- Se tienen que definir.
- Se llaman con el nombre y no tienen argumentos.
	- El **argumento** es la asignación (después del **=**)

-  ***Getter***: es una función para establecer el valor en la propiedad de un objeto.
- ***Setter***: ss una función para cambiar el valor en la propiedad de un objeto.

- <u>Ejemplo:</u>
	```js
		const persona = {
			_edad: 0,
			set edad (nuevaEdad) {
				if(nuevaEdad > 0){
					this._edad = nuevaEdad;
				}else{
					console.log('Edad no valida')
				}
			},
			get edad () {
				return this._edad;
			}
		}
		
		console.log(persona.edad)  // 0
		pesrona.edad = 25;  //25
		persona.edad = -2;  //Edad no validad
		console.log(persona.edad)  // 25
	```

# Bucles en los objectos - ``in``<a name='bucles'></a>
- Para saber si existe una propiedad se usa la palabra clave ``in``
	- ``(propiedad in objectName)``
- Para ver todas las propiedades de un objeto, se recorre con un *loop / for* como los [[3. Bucles sobre arrays ➰➰➰]]:
	 ```js
		for (const key in objectName){
			...
		}
	```
- Para ver los valores de las propiedades:
	 ```js
		for (const key in objectName){
			return objectName[key];
		}
	```

## Acceder a los objectos de un array
- Si tenemos un array de objetos hay dos formas de acceder a los objetos:
	1. Bucle *for*
	2. Bucle *for - of*

### *for of*<a name='of'></a>
- Recorrere los elementos.
-  <u>Ejemplo:</u>
	```js
	for (let obj of array){
		console.log(`El elemento es ${obj});
	}
	```