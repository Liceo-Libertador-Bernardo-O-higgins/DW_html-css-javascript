
# 📚 Curso de Desarrollo Web: HTML, CSS y JavaScript

## ✨ Descripción
Este curso está diseñado para estudiantes que se inician en el desarrollo web. A lo largo de las unidades se trabajará con **HTML**, **CSS** y **JavaScript**, abarcando desde lo más básico hasta la creación de páginas web interactivas con formularios, modales y efectos dinámicos.

---

## 📅 Unidades y Contenidos

### 🔹 Unidad 1: Introducción a HTML
**Contenidos:**
- Estructura básica (`<!DOCTYPE html>`, `<html>`, `<head>`, `<body>`).
- Etiquetas esenciales: `<h1>`, `<p>`, `<a>`, `<img>`, `<ul>`, `<li>`, `<div>`, `<span>`, etc.
- Atributos: `href`, `src`, `alt`, `id`, `class`.

**Actividad:** Crear una página personal con nombre, foto y lista de pasatiempos.

```html
<!-- Página personal -->
<h1>Juan Pérez</h1>
<img src="foto.jpg" alt="Foto" width="200">
<ul>
  <li>Programar</li>
  <li>Leer</li>
  <li>Fútbol</li>
</ul>
```

---

### 🔹 Unidad 2: Estilos con CSS
**Contenidos:**
- Tipos de CSS: en línea, interno, externo.
- Propiedades básicas: `color`, `background`, `font-family`, `margin`, `padding`, `border`.

**Actividad:** Aplicar estilos a la página personal.

```css
/* Estilos generales */
body {
  background-color: #f0f0f0;
  font-family: Arial;
}
h1 {
  color: navy;
}
```

---

### 🔹 Unidad 3: Introducción a JavaScript
**Contenidos:**
- `script`, `alert`, `prompt`, `console.log`.
- Variables (`let`, `const`), tipos de datos, operadores.

**Actividad:** Agregar botón que salude al usuario.

```javascript
// Función para saludar al usuario
function saludar() {
  let nombre = prompt("¿Cómo te llamas?");
  alert("Hola " + nombre);
}
```

---

### 🔹 Unidad 4: Interacción con el DOM
**Contenidos:**
- `getElementById`, `innerHTML`, `value`.
- Eventos como `onclick`.

**Actividad:** Calculadora de suma.

```html
<!-- Inputs y botón para sumar -->
<input type="number" id="num1">
<input type="number" id="num2">
<button onclick="sumar()">Sumar</button>
<p id="resultado"></p>
<script>
  function sumar() {
    let a = parseInt(document.getElementById("num1").value);
    let b = parseInt(document.getElementById("num2").value);
    document.getElementById("resultado").innerHTML = "Resultado: " + (a + b);
  }
</script>
```

---

### 🔹 Unidad 5: Formularios HTML + Validación
**Contenidos:**
- Elementos: `<form>`, `<input>`, `<label>`, `<textarea>`, `<select>`, `<option>`.
- Atributos: `required`, `placeholder`, `type`, `name`, `id`, `for`.
- Validación con HTML y JS.

**Actividad:** Formulario de contacto con validación.

```html
<!-- Formulario de contacto -->
<form onsubmit="return validarFormulario()">
  <label for="nombre">Nombre:</label>
  <input type="text" id="nombre" required>
  <button type="submit">Enviar</button>
</form>
<script>
  function validarFormulario() {
    let nombre = document.getElementById('nombre').value;
    if (nombre === "") {
      alert("Campo obligatorio");
      return false;
    }
    return true;
  }
</script>
```

---

### 🔹 Unidad 6: Modales (Ventanas Emergentes)
**Contenidos:**
- CSS: `display`, `position`, `z-index`, `background`.
- Mostrar/Ocultar con JavaScript.

**Actividad:** Mostrar mensaje en modal.

```html
<!-- Modal simple -->
<button onclick="abrirModal()">Abrir Modal</button>
<div id="miModal" style="display:none; position:fixed; background:#fff; border:1px solid #000; padding:20px;">
  <p>Este es un modal</p>
  <button onclick="cerrarModal()">Cerrar</button>
</div>
<script>
  function abrirModal() {
    document.getElementById("miModal").style.display = "block";
  }
  function cerrarModal() {
    document.getElementById("miModal").style.display = "none";
  }
</script>
```

---

### 🔹 Unidad 7: Estilos Avanzados y Responsive Design
**Contenidos:**
- Pseudoclases (`:hover`, `:focus`).
- Transiciones (`transition`), animaciones (`@keyframes`).
- Media Queries y diseño adaptable.
- Flexbox y Grid.

**Actividad:** Menú responsive con cambios de color al pasar el mouse.

```css
/* Menú adaptable */
nav a:hover {
  background-color: lightblue;
}
@media (max-width: 600px) {
  nav {
    flex-direction: column;
  }
}
```

---

### 🔹 Unidad 8: JavaScript Dinámico
**Contenidos:**
- `addEventListener`, `classList`.
- Temporizadores (`setTimeout`, `setInterval`).
- Arrays y navegación entre elementos.

**Actividad:** Galería de imágenes.

```html
<!-- Galería de imágenes con botones -->
<img id="galeria" src="img1.jpg" width="300">
<button onclick="siguiente()">Siguiente</button>
<script>
  let imagenes = ["img1.jpg", "img2.jpg"];
  let indice = 0;
  function siguiente() {
    indice = (indice + 1) % imagenes.length;
    document.getElementById("galeria").src = imagenes[indice];
  }
</script>
```

---

### 🧪 Proyecto Final
**Objetivo:** Crear una web completa que integre:
- Menú navegable.
- Formulario validado.
- Modal interactivo.
- Diseño adaptable a dispositivos móviles.

---

## 📂 Recursos adicionales
- [MDN Web Docs (HTML)](https://developer.mozilla.org/es/docs/Web/HTML)
- [MDN Web Docs (CSS)](https://developer.mozilla.org/es/docs/Web/CSS)
- [MDN Web Docs (JavaScript)](https://developer.mozilla.org/es/docs/Web/JavaScript)

---

## 📈 Evaluación sugerida
- ✅ Rúbricas por unidad (HTML, CSS, JS).
- ✅ Presentación final del proyecto.
- ✅ Autoevaluación y coevaluación del trabajo en grupo.

---

## ✍️ Autor
**Profesor de Programación y Educación Física**  
📍 Chile | 💻 Educación Técnica Profesional  
