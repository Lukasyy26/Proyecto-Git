# JavaScript moderno

Desde ES6 (2015) JavaScript incorpora funcionalidades que hacen el código más claro y seguro.

## Variables: let y const

```javascript
const nombre = "Ana";   // no se puede reasignar
let edad = 20;          // se puede reasignar
edad = 21;
```

Se evita `var` por su comportamiento confuso con el ámbito.

## Funciones flecha

```javascript
const sumar = (a, b) => a + b;
console.log(sumar(2, 3)); // 5
```

## Template literals

```javascript
const saludo = `Hola, ${nombre}. Tienes ${edad} años.`;
```

## Desestructuración y spread

```javascript
const usuario = { nombre: "Ana", ciudad: "Gijón" };
const { nombre, ciudad } = usuario;

const numeros = [1, 2, 3];
const ampliada = [...numeros, 4, 5];
```

## Módulos

```javascript
// utilidades.js
export function duplicar(n) {
  return n * 2;
}

// main.js
import { duplicar } from "./utilidades.js";
```

## Asincronía: async/await y fetch

```javascript
async function obtenerUsuarios() {
  try {
    const respuesta = await fetch("https://jsonplaceholder.typicode.com/users");
    const datos = await respuesta.json();
    console.log(datos);
  } catch (error) {
    console.error("Error al obtener los datos:", error);
  }
}
```

## Métodos de arrays

- `map()`: transforma cada elemento.
- `filter()`: se queda con los que cumplen una condición.
- `reduce()`: reduce el array a un solo valor.

```javascript
const pares = [1, 2, 3, 4].filter(n => n % 2 === 0); // [2, 4]
```
