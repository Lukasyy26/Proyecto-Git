# CSS avanzado

CSS permite crear diseños complejos, adaptables y con animaciones sin necesidad de JavaScript.

## Flexbox

Sirve para organizar elementos en una dimensión (fila o columna).

```css
.menu {
  display: flex;
  justify-content: space-between;
  align-items: center;
  gap: 1rem;
}
```

- `justify-content`: reparte los elementos en el eje principal.
- `align-items`: los alinea en el eje secundario.
- `gap`: espacio entre elementos.

## CSS Grid

Sirve para diseños en dos dimensiones (filas y columnas).

```css
.galeria {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 1rem;
}
```

## Variables CSS

Permiten reutilizar valores en toda la hoja de estilos.

```css
:root {
  --color-principal: #1e88e5;
  --espaciado: 16px;
}

.boton {
  background-color: var(--color-principal);
  padding: var(--espaciado);
}
```

## Media queries (diseño responsive)

```css
@media (max-width: 768px) {
  .galeria {
    grid-template-columns: 1fr;
  }
}
```

## Transiciones y animaciones

```css
.boton {
  transition: transform 0.3s ease;
}
.boton:hover {
  transform: scale(1.1);
}

@keyframes aparecer {
  from { opacity: 0; }
  to   { opacity: 1; }
}
.tarjeta {
  animation: aparecer 1s ease-in;
}
```

