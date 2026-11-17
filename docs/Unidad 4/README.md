# Unidad 4 — KEMSA-V

## Sistema de Gestión de Eventos

Entrega del proyecto funcional en navegador. El archivo principal es [index.html](./index.html).

### Cómo abrir

- **En línea:** una vez activado GitHub Pages, visita https://karlabucio.github.io/KEMSA-V/ (el inicio redirige a esta unidad).
- **Localmente:** descarga `index.html` y ábrelo con Chrome, Edge u otro navegador moderno.

### Funciones implementadas

- Panel de inicio con accesos a eventos, próximos eventos, clientes y personal.
- Registro, consulta, edición y eliminación de clientes, personal y eventos.
- Eventos con fecha, hora, estado, ubicación, cliente, encargado, invitados y presupuesto.
- Formulario de especificaciones con servicios solicitados (flores, música, fotografía, decoración, etc.).
- Calendario mensual interactivo, selección directa de mes y año, indicadores de colores según estado y edición de eventos.
- Filtros y búsqueda.

### Organización técnica

Esta entrega conserva el **código completo en un solo HTML**, porque permite abrir la demostración directamente sin instalar dependencias, servidores ni Python.

| Capa | Implementación actual |
| --- | --- |
| Interfaz visual (frontend) | HTML y CSS incrustados en `index.html` |
| Lógica del sistema | JavaScript incrustado en `index.html` |
| Persistencia local | `localStorage` del navegador |
| Backend/API | No implementado en esta versión |
| Base de datos compartida | No implementada; `localStorage` no es una BD de servidor |

### Consideraciones para la evaluación

Los datos se guardan localmente **por navegador y por origen**. No se sincronizan entre dispositivos; limpiar los datos del sitio puede eliminar los registros guardados. El archivo incluye datos de demostración. Evita almacenar información personal real o confidencial en esta demostración pública. La publicación mediante GitHub Pages aloja solo los archivos estáticos: **no crea un backend ni una base de datos**.

### Evidencias sugeridas

1. Pantalla de inicio y estadísticas.
2. Registro y edición de clientes y personal.
3. Creación y cambio de estado de un evento.
4. Selección de servicios en especificaciones.
5. Calendario con búsqueda de mes/año y eventos por color.

### Nota de despliegue

Si no abre la URL pública, en **Settings → Pages** configura **Deploy from a branch → main → /(root)** o **main → /docs**, y guarda. Este repositorio contiene archivos de inicio en ambas ubicaciones que redirigen al proyecto de Unidad 4. La activación de Pages requiere acceso de administración a GitHub.
