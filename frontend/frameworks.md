# Frameworks frontend

Un framework ofrece una estructura y herramientas para construir interfaces complejas de forma organizada, dividiéndolas en componentes reutilizables.

## React

Biblioteca creada por Meta. Basada en componentes y en JSX.

```jsx
function Saludo({ nombre }) {
  return <h1>Hola, {nombre}</h1>;
}
```

- Muy extendida y con gran ecosistema.
- [Documentación oficial](https://react.dev/)

## Vue

Framework progresivo, fácil de aprender.

```html
<template>
  <h1>Hola, {{ nombre }}</h1>
</template>

<script>
export default {
  data() {
    return { nombre: "Ana" };
  }
};
</script>
```


