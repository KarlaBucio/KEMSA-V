# KEMSA-V — Sistema de Gestión de Eventos

Proyecto académico de la materia **Gestión de Proyectos de Software**.

**Estado actualizado al 17 de noviembre de 2026:** versión demostrativa funcional en navegador, con los módulos de eventos, clientes, personal y calendario. Se encuentra en etapa de **integración y validación**, con funciones adicionales y persistencia compartida aún pendientes.

**[Abrir la aplicación web (GitHub Pages)](https://karlabucio.github.io/KEMSA-V/)** · **[Ver código de la Unidad 4](docs/Unidad%204/index.html)** · **[Documentación de la Unidad 4](docs/Unidad%204/README.md)**

> El enlace web requiere que GitHub Pages esté habilitado y haya finalizado su despliegue. La disponibilidad pública del sitio no se da por verificada en este documento.

## Descripción

KEMSA-V es un sistema de gestión para empresas dedicadas a la organización de eventos. Su finalidad es concentrar el registro y seguimiento de eventos, clientes, responsables, fechas y requerimientos en una sola interfaz.

El alcance general del proyecto también contempla servicios, cotizaciones, contratos y pagos, que no deben confundirse con funciones ya implementadas en la demostración de la Unidad 4.

## Estado del proyecto

| Componente o actividad | Estado al 17/11/2026 | Observaciones |
| --- | --- | --- |
| Interfaz web principal | Implementado en la demostración | Panel inicial y navegación |
| Gestión de clientes | Implementado en la demostración | Alta, consulta, edición y eliminación |
| Gestión de personal | Implementado en la demostración | Alta, consulta, edición y eliminación |
| Gestión de eventos | Implementado en la demostración | Registro, consulta, edición, eliminación, responsable y estados |
| Especificaciones de eventos | Implementado en la demostración | Invitados, montaje, flores, música, fotografía, decoración y otros servicios |
| Calendario interactivo | Implementado en la demostración | Vista mensual, selección de mes/año, colores por estado, creación y edición |
| Búsquedas y filtros | Implementado en la demostración | Consultas de registros y eventos |
| Persistencia de registros en navegador | Implementado | Mediante `localStorage`; datos separados por navegador |
| Backend/API y conexión a BD compartida | No integrados en esta demostración | Requieren implementación o integración y pruebas |
| Cotizaciones, contratos y pagos | Alcance previsto | Sin implementación acreditada por el HTML entregado |
| Pruebas integrales y validación multiusuario | Pendiente de acreditar | La revisión del código no sustituye pruebas funcionales completas |
| Publicación web | Archivos preparados | Verificar activación y despliegue correcto de GitHub Pages |

### Avances de la Unidad 4

- Revisión del proyecto y preparación de la versión de entrega.
- Simplificación de los formularios de clientes, personal y eventos.
- Incorporación del formulario de especificaciones y servicios de eventos.
- Implementación de calendario con colores para **Próximo, En curso, Pospuesto, Cancelado y Finalizado**.
- Selección directa de mes y año en el calendario.
- Accesos directos desde las tarjetas del panel de inicio.
- Organización y subida del proyecto a `docs/Unidad 4/`.
- Creación del README específico de la Unidad 4.
- Preparación de los archivos de inicio para acceder mediante GitHub Pages.

**[Consultar las tareas registradas de la Unidad 4 (Issues #21–#29)](https://github.com/KarlaBucio/KEMSA-V/issues?q=is%3Aissue+Unidad+4)**

Estas nueve actividades están registradas como cerradas en GitHub Issues. Esto no implica que todas las fases generales o los módulos futuros estén terminados.

## Tecnologías de la versión demostrativa

- **HTML5:** estructura de las páginas y formularios.
- **CSS3:** presentación visual y diseño adaptable.
- **JavaScript:** navegación, calendario, filtros y operaciones sobre registros.
- **localStorage:** almacenamiento local en el navegador.
- **Git y GitHub:** versionado y organización de entregables.
- **GitHub Pages:** opción de alojamiento de la versión estática.

La demostración se entrega en un archivo HTML que integra la presentación y la lógica de JavaScript. **No utiliza actualmente una API de servidor ni una base de datos compartida.** El diseño o desarrollo de base de datos y backend del proyecto general debe validarse e integrarse por separado.

## Instalación y ejecución

### Abrir en línea

Acceder a **https://karlabucio.github.io/KEMSA-V/** una vez publicado el sitio en GitHub Pages.

### Abrir localmente

1. Abrir [`docs/Unidad 4/index.html`](docs/Unidad%204/index.html).
2. Descargar el archivo HTML.
3. Abrirlo en un navegador moderno (Chrome o Edge).

No se requiere instalar Python, dependencias ni un servidor para esta demostración estática.

**Nota:** la información se conserva por navegador mediante `localStorage`. Los datos no se sincronizan entre dispositivos y pueden perderse al borrar el almacenamiento del sitio. Se incluyen registros de ejemplo; no se recomienda ingresar información personal confidencial en la demo pública.

## Usuarios del sistema

Usuarios contemplados en el alcance general:

- Empresas dedicadas a la organización y gestión de eventos.
- Empleados.
- Clientes.

La interfaz demostrativa actual representa una vista de administración. No debe interpretarse como un sistema completo de cuentas, roles, autenticación y permisos diferenciados.

## Integrantes y roles

- **José Vidal López Casimiro** — Backend y líder designado.
- **Saúl García Galván** — Base de datos.
- **Edgar Omar García Pardo** — Backend.
- **Mónica Nayeli Rodríguez Peña** — Frontend.
- **Karla Paola Bucio López** — Frontend.

Los roles provienen de la organización original del proyecto; no constituyen asignación individual de las nuevas tareas de la Unidad 4.

## Alcance general

El sistema contempla consulta y organización de eventos; registro y consulta de clientes; servicios como decoración, música, fotografía, catering y mobiliario; cotizaciones, precios y servicios contratados; y organización de fechas para evitar conflictos de horarios.

Se restringirá la visualización de datos sensibles, contraseñas, datos personales innecesarios, información de otros clientes y parámetros técnicos exclusivos del administrador **cuando se implementen los controles de acceso correspondientes**. La demostración actual no ofrece autenticación ni control de acceso por usuario.

## Forma de trabajo

Lineamientos establecidos para el proyecto:

- La rama principal es `main`.
- Cada tarea se desarrolla en una rama independiente.
- Cada cambio debe tener un commit descriptivo.
- Antes de integrar una tarea a `main`, se debe abrir un Pull Request y solicitar revisión de otro integrante.
- La evidencia de cada tarea debe quedar ligada a su commit o Pull Request.
- Los cambios al alcance, fechas o línea base deberán registrarse mediante el procedimiento de control de cambios.

## Fases del proyecto (cronograma original)

1. Requerimientos y alcance — 10 al 18 de septiembre.
2. UML, casos de uso, BD y prototipos — 19 al 30 de septiembre.
3. Base de datos funcional — 1 al 9 de octubre.
4. Backend, CRUD y lógica del sistema — 10 al 30 de octubre.
5. Frontend e interfaces funcionales — 31 de octubre al 13 de noviembre.
6. Integración del sistema — 14 al 20 de noviembre.
7. Pruebas y correcciones — 21 al 27 de noviembre.
8. Documentación y presentación — 28 de noviembre al 4 de diciembre.

**Importante:** las fechas anteriores corresponden al plan inicial, no a una confirmación de que cada fase se completó. Al 17 de noviembre, el plan sitúa al proyecto en el periodo de integración; la integración real de backend y base de datos no está demostrada por esta entrega estática.

## Próximas actividades

- Verificar que la URL de GitHub Pages abra correctamente el sistema.
- Probar exhaustivamente altas, modificaciones, eliminaciones, filtros y calendario.
- Evaluar e integrar el backend y la base de datos compartida.
- Revisar validación de datos, seguridad, autenticación y gestión de usuarios si el alcance final lo requiere.
- Implementar o integrar los módulos de cotizaciones, contratos y pagos previstos en el alcance.
- Documentar resultados de pruebas, errores corregidos y avances de integración.

## Entregables

- **[Unidad 4: proyecto funcional y documentación](docs/Unidad%204/)**.
- **[Seguimiento de actividades en Issues](https://github.com/KarlaBucio/KEMSA-V/issues)**.
- **[Demostración web](https://karlabucio.github.io/KEMSA-V/)**, mediante GitHub Pages.
