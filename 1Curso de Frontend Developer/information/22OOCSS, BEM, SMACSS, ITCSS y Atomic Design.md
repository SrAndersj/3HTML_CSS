# OOCSS

## PRINCIPIOS

- Separar la estructura y la piel:

  - **Objeto**: Estructura base.
  - **Máscara**: Elementos visuales iguales.

- Separar el contenedor del contenido:
  - Contenedores no deben afectar el estilo del contenido.

# BEM (Block Element Modifier)

BEM es una metodología de nomenclatura para clases en HTML y CSS. Está diseñada para hacer que el desarrollo de interfaces sea más claro y comprensible, facilitando la reutilización de código y reduciendo el acoplamiento entre los estilos y la estructura HTML.

- **Bloque**: El componente independiente que puede ser reutilizado. Representa el nivel más alto de abstracción de un nuevo componente.
- **Elemento**: Una parte del bloque que tiene sentido en el contexto del bloque. Estos son subcomponentes que no pueden usarse de manera independiente fuera del bloque.
- **Modificador**: Una bandera o configuración que cambia la apariencia o comportamiento del bloque o elemento para una variante más específica o de uso especial.

https://platzi.com/blog/bem/

# SMACSS (Scalable and Modular Architecture for CSS)

SMACSS es una metodología de diseño para crear códigos CSS mantenibles y escalables. Divide las reglas de estilo en cinco categorías:

- **Base**: Estilos predeterminados para elementos HTML, como `body`, `input`, `button`, que no clasificamos con clases específicas.
- **Layout**: Estilos que dividen la página en secciones; incluyen cabeceras, pies de página, y otros contenedores.
- **Module**: Los módulos son los componentes reutilizables y modulares de la construcción de la página, como barras de navegación y sliders.
- **State**: Estilos que describen cómo los módulos o layouts se verán cuando estén en un estado particular (como `.isActive` o `.isDisabled`).
- **Theme**: Estilos específicos para dar apariencia y sensación distintivas. Por ejemplo, los temas pueden incluir colores o fuentes que cambian entre diferentes versiones del diseño.

La combinación de estas categorías resulta en una arquitectura robusta y predecible para su CSS.

# ITCSS (Inverted Triangle CSS)

ITCSS es una arquitectura CSS que ayuda a organizar tus hojas de estilo de una manera más eficiente y mantenible. Se basa en la idea de un triángulo invertido que representa cómo deberían ser estructurados los estilos, desde los más genéricos hasta los más específicos:

- **Ajustes**: Configuración global y variables de diseño (como colores y fuentes).
- **Herramientas**: Mixins y funciones que se utilizan en todo el proyecto.
- **Genéricos**: Estilos de bajo nivel, como reset o normalize.
- **Elementos**: Estilos predeterminados para elementos HTML sin clases.
- **Objetos**: Patrones de diseño como el sistema de cuadrícula.
- **Componentes**: Estilos específicos de UI para componentes.
- **Utilidades**: Clases de utilidad que tienen una alta especificidad y se pueden usar para sobrescribir cualquier cosa si es necesario.

A medida que te mueves hacia abajo en el triángulo, la especificidad aumenta, al igual que la magnitud (cantidad de código) y la claridad.

# Atomic Design

El diseño atómico es una metodología para crear sistemas de diseño de interfaces de manera sistemática, enfocándose en la creación y combinación de interfaces consistentes y reutilizables.

- **Átomos**: Los bloques de construcción más básicos, como etiquetas HTML como un botón, un input de texto o un enlace.
- **Moléculas**: Grupos de átomos que funcionan juntos como una unidad, como un formulario de búsqueda con un input y un botón.
- **Organismos**: Conjuntos de moléculas que forman una sección de una interfaz, como un encabezado compuesto por el logo, navegación y formulario de búsqueda.
- **Plantillas**: Combinaciones de organismos que forman la estructura de una página.
- **Páginas**: Instancias específicas de plantillas que muestran cómo se verá la UI con contenido real en el contexto final.
