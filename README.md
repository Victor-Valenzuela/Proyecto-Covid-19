# Cierre Modulo 4 "Desarrollo de aplicaciones web".

Descripción general del proyecto

A nivel mundial nos encontramos en una pandemia, que ha afectado a casi todo el mundo y todas las personas están intentando aportar su granito de arena, tú también quieres hacerlo con las habilidades de desarrollador web que has adquirido en Desafío Latam.

Te has propuesto construir un sitio web que informe a la gente la situación actual (contagiados, muertos y recuperados) del Covid-19 por país. En cuanto a la magnitud del proyecto, el enfoque principal será el de consumir diferentes APIs con la información relacionada al Covid-19, esta se deberá mostrar en gráficos y tablas para que los usuarios que visiten la página tengan una visión general y fácil de entender.

El entorno de trabajo será en un proyecto realizado con JavaScript en Node.js, que nos permitirá generar un ambiente real de trabajo, en donde el Front de la aplicación deberá consumir las APIs mediante AJAX con JavaScript o jQuery. Para manejar la autenticación del usuario se tendrá que persistir el JWT entregado por el backend a través del localStorage o similar.

Para llevar a cabo el proyecto deberás:
- Generar y preparar los elementos de HTML para poder ser accedidos desde JavaScript o jQuery.
- Utilizar AJAX para obtener los datos desde el backend de la aplicación.
- Utilizar librerías externas para llegar a los requerimientos, específicamente una librería para la creación de gráficos.
- Manipular el DOM con JavaScript o jQuery.
- Usar la lógica de programación para filtrar y recorrer arrays de objetos con la información.

Hito 1 - Situación Mundial
Requerimientos
1. Crear una estructura básica con html para el proyecto y cargar la librería de bootstrap o similar, además de Jquery. (1 Punto)
2. Consumir la API http://localhost:3000/api/total con JavaScript o jQuery. (1 Punto)
3. Desplegar la información de la API en un gráfico de barra que debe mostrar sólo los países con más de 10000 casos activos. (4 Puntos)
4. Desplegar toda la información de la API en una tabla. (1 Punto)
5. Cada fila de la tabla debe incluir un link que diga "ver detalle", al hacer click levante un modal y muestre los casos activos, muertos, recuperados y confirmados en un gráfico, para obtener esta información debes llamar a la API http://localhost:3000/api/countries/{country} al momento de levantar el modal. (3 Puntos)

Hito 2 - Situación de Chile
Requerimientos
1. Crear una barra de navegación en la parte superior con una opción que diga “Home” y otra de “Iniciar sesión”. (0.5 Puntos)
2. Al hacer click en Iniciar sesión se debe levantar un modal con un formulario que le pida al usuario ingresar un correo y una contraseña. (0.5 Puntos)
3. Implementar la lógica para obtener el JWT cuando se ingrese el correo y contraseña a través del formulario. (3 Puntos)
- Llamar a la API para obtener el JWT.
- Persistir el JWT.
- Cuando exista un JWT, se debe ocultar la opción del menú que dice Iniciar sesión, se debe agregar una que diga Situación Chile y otra de Cerrar sesión.
4. Al hacer click sobre la opción Situación Chile, se debe mostrar una nueva página donde se añadirá un gráfico y se debe ocultar el gráfico de todos los países con la
tabla. (1 Punto)
5. Al hacer click en la opción Situación Chile, se debe llamar a las siguientes APIs. (2 Puntos)
- http://localhost:3000/api/confirmed.
- http://localhost:3000/api/deaths.
- http://localhost:3000/api/recovered
6. En un sólo gráfico de línea se debe mostrar la información obtenida de las APIs del punto 5. (2 Puntos)
7. Al hacer click sobre el link Cerrar sesión del menú se debe volver al estado inicial de la aplicación, eliminar el token y ocultar los link de Situación Chile y Cerrar sesión, además de volver a mostrar Iniciar sesión. (1 Punto)
