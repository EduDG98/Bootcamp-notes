# API Storage 🍪

- Es una fomra de almacenamiento web.
- Hay dos tipos de almacenamiento / _Storage_:
  - **_session_** --> la información alamacenada se eleimina al terminar la sesión de la pág. web.
  - **_local_** --> a información alamacenada se eleimina cuando uno quiere.

# Métodos:

- `getItem('clave')` --> coger la clave para almacenarla en una variable JS.
- `setItem('clave', valor)` --> crear una clave con un valor.
- `removeItem('clave')` --> eliminar una clave.
- `clear()` --> borrar todas las claves
- `key(n)` --> devuelve la clave _n_ almacenada.

# _Local Storage_ & _Session Storage_

- Es un Objeto _Storage_.
- <u>Ejemplo:</u>
  ```js
  localStorage.setItem("accepted", true);
  const butonYes = localStorage.getItem("accepted"); // true
  localStorage.removeItem("accepted");
  localStorage.clear();
  ```
