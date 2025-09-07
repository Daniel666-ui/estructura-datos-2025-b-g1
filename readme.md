# 📚 Sistema de Gestión de Biblioteca — Unidad 1

## 📌 Descripción
Este proyecto implementa un **sistema de gestión de biblioteca** en Java utilizando los conceptos de la Unidad 1 de Estructuras de Datos:
- Arrays 1D y 2D para el catálogo de libros y la disponibilidad en sucursales.
- Lista enlazada simple para los préstamos activos.
- Lista doblemente enlazada para el historial de operaciones.
- Programación estructurada con métodos, menús (`switch`) y bucles (`while/for`).

El sistema permite: registrar libros, eliminarlos (baja lógica), buscar por título, prestar y devolver libros, ver préstamos activos y recorrer el historial hacia adelante y atrás.

---

## 🧩 Razones de elección de estructuras y complejidad

### Catálogo — `Libro[]` (array 1D)
- **Razón:** Se pidió usar arrays fijos para practicar inserción, búsqueda y control de índices.
- **Operaciones clave:**
  - Alta (insertar si hay espacio): **O(1)**.
  - Búsqueda por título (lineal): **O(n)**.
  - Baja lógica: **O(n)** (buscar y marcar inactivo).

### Disponibilidad por sucursal — `int[][]` (matriz 2D)
- **Razón:** Representar el stock de libros en varias sucursales.
- **Operación:** Actualización de stock: **O(1)**.

### Préstamos — Lista enlazada simple (`Prestamo`)
- **Razón:** Practicar nodos y enlaces simples para manejar préstamos activos.
- **Operaciones clave:**
  - Inserción al final: **O(n)**.
  - Eliminación (devolución): **O(n)**.

### Historial — Lista doblemente enlazada (`Historial`)
- **Razón:** Permite recorrer operaciones hacia adelante y hacia atrás.
- **Operaciones clave:**
  - Inserción al final: **O(1)**.
  - Recorridos: **O(n)**.

---

## ▶️ Cómo compilar y ejecutar

### Desde la terminal
1. Guardar el archivo como `Biblioteca.java`.
2. Compilar:
   ```bash
   javac Biblioteca.java
