# 🛒 Tienda Online JS - Evaluación de Portafolio

Este proyecto consiste en una aplicación de **E-commerce (SPA)** desarrollada con JavaScript Vanilla, aplicando conceptos avanzados como **Programación Orientada a Objetos (POO)**, manejo del **DOM** y consumo de **APIs REST**.

El objetivo es demostrar la capacidad de construir una interfaz interactiva y funcional que gestione datos dinámicos, simulando un carrito de compras real.

## 🚀 Características Principales

* **Carga Dinámica de Productos:** Los productos no están escritos en el HTML, sino que se obtienen en tiempo real desde una API externa.
* **Carrito de Compras:** Lógica para agregar productos, calcular el total automáticamente y eliminar ítems.
* **POO (Programación Orientada a Objetos):** Uso de Clases (`class Producto`) para modelar los datos y encapsular la lógica de renderizado.
* **Persistencia de Estado:** Gestión de arrays en memoria para el catálogo y el carrito.
* **Diseño Responsivo:** Interfaz adaptada a móviles y escritorio utilizando **Bootstrap 5**.

## 🛠️ Tecnologías y Conceptos Aplicados

* **JavaScript (ES6+):**
    * `Classes` & `Constructors`.
    * `Async / Await` & `Fetch API` para asincronía.
    * `Arrow Functions` y `Destructuring`.
    * `Template Literals` para inyección de HTML.
* **HTML5 & CSS3:** Estructura semántica.
* **Bootstrap 5:** Framework de estilos para agilizar el diseño (Grid, Cards, Badges).
* **API Externa:** [FakeStoreAPI](https://fakestoreapi.com/) (Datos reales de productos).

## 📂 Estructura del Proyecto
```text
/proyecto-ecommerce
  ├── index.html           # Interfaz de usuario (Grid y Carrito)
  ├── app.js               # Lógica del negocio (Clases, Fetch, Eventos)
  ├── README.md            # Documentación del proyecto
  └── assets
      └── css
          └── style.css    # Estilos personalizados y efectos hover
```

## ⚙️ Instalación y Uso
Este proyecto funciona directamente en el navegador sin necesidad de compiladores ni bundlers.

* **Clonar el repositorio:**
``` bash
git clone https://github.com/kserey/skillnest-m4-portafolio
```
* **Ejecutar:**
  * Abre el archivo index.html en tu navegador.
  * Al cargar, verás el catálogo de productos obtenido de la API.

## 🔍 Detalles de Implementación
**Clase Producto**
Se implementó una clase con un método renderizarTarjeta() que devuelve el HTML necesario para cada ítem, manteniendo el código limpio y modular.

```JavaScript
class Producto {
    constructor({ title, price, ... }) { ... }
    renderizarTarjeta() { return `...html...`; }
}
```

**Consumo de API** 
Se utilizó async/await para gestionar la latencia de red y un bloque try/catch para manejar posibles errores de conexión, mostrando una alerta visual al usuario si la API falla.

## ✒️ Autor
Irina Serey - Desarrollador Full Stack en formación
