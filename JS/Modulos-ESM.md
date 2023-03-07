# Módulos ESM 💾

## Exports e imports

- Se pueden **exportar** funciones / constantes / módulo añadiendo `export` delante de ellos.
- Y luego **importarlos** en otro archivo JS con:
  - `import { ... } from './modules/...'`
  - Se le puede cambiar el nombre a lo que se importa con `as`:
    - `import { max as maximo } from './modules/mathematical.js'`

## Otras formas exportar

- Exportar todos los elementos al final
  - `export default { ... , ... }`
- **No** se recomienda.

## Imports node_modules

- Si se importa algo que no empieza por `./` se trata de un paquete.
- Para poder importar un paquete tiene que estar instalado previamente

## Importación `*`

- Importa todo lo que en la ruta en el objeto definido
  - `import * as object from './modules/...'`

## Importar código literal

- Importa el codigo que hay en la ruta y lo ejecuta.
  - `import './modules/fichero.js'`

## Forma vieja de importar y exportar

- Para importar se usaba `require(' ... ')`
- Para exportar `module.export = { PI, min, max}`
