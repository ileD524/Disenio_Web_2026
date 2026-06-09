# Preguntas Teóricas a resolver

## Presentaciones
1. **¿Aplicación Web = Sitio Web? ¿Por qué?** 
A diferencia de lo que podríamos considerar un sitio web tradicional estático, una aplicación web es un software codificado en un lenguaje soportado por los navegadores en el que se confía su ejecución al navegador. Además, pueden generar páginas web interactivas con contenido dinámico (orientadas a la presentación) o implementar el punto final de un servicio web (orientadas al servicio).

2. **¿A qué nos referimos cuando hablamos de “cliente” en desarrollo web?**
En la web, el "cliente" principal son los navegadores (o browsers) que solicitan información al servidor. En una arquitectura Cliente/Servidor, el cliente es quien inicia las solicitudes, teniendo un papel activo en la comunicación, para luego esperar y recibir las respuestas del servidor. Normalmente, el cliente es la parte que interactúa de forma directa con los usuarios finales a través de una interfaz gráfica.

3. **¿A qué nos referimos cuando hablamos de lenguaje del lado del cliente? Mencione ejemplos**
Son aquellos lenguajes que son totalmente independientes del servidor y que pueden ser "digeridos" e interpretados directamente por el navegador del usuario sin necesitar un pretratamiento. Ejemplos de lenguajes del lado del cliente son HTML, JavaScript, Applets de Java y CSS.

4. **¿A qué nos referimos cuando hablamos de lenguaje del lado del servidor? Mencione ejemplos**
Son los lenguajes que son reconocidos, ejecutados e interpretados por el propio servidor, y cuyo resultado se envía luego al cliente en un formato que éste pueda comprender. Algunos ejemplos son CGI (que se suele escribir en Perl, C, C++ o Visual Basic), ASP.net, PHP y Java Server Pages (JSP).

5. **¿Puedo conectarme a una base de datos utilizando HTML?**
HTML es un lenguaje de la Capa de Presentación que sirve únicamente para indicarle al navegador dónde colocar texto, imágenes o vídeo. La conexión, el flujo de procesos y la grabación de información en una base de datos ocurren en la "Capa de negocios" y la "Capa de datos", para lo cual se necesita programación del lado del servidor. Por lo tanto, no te podés conectar a una base de datos usando solo HTML.

## Web Estáticas y Dinámicas
1. **¿Qué es una página web dinámica? Mencione sus características**
Una página web dinámica es un documento en línea que genera contenido en tiempo real y varía según la interacción del usuario, la hora o datos externos.

    **Características principales de las páginas web dinámicas:**
    - **Interactividad Elevada:** Los usuarios pueden interactuar a través de formularios, carritos de compra, filtros de búsqueda y comentarios.
    - **Contenido en Tiempo Real:** El sitio se actualiza automáticamente según el comportamiento del usuario o cambios en la base de datos.
    - **Personalización:** Muestran información específica para cada visitante (ej. "Hola, [Nombre]", historial de compras).
    - **Uso de Base de Datos y Servidor:** Requieren tecnologías del lado del servidor (PHP, ASP.NET, Python) y sistemas de gestión de contenido (CMS) para gestionar grandes cantidades de información.
    - **Funcionalidad Avanzada:** Permiten automatizar tareas y gestionar sistemas complejos como sesiones de usuario o pasarelas de pago.

2. **Nombre 3 ejemplos de ellas**
    - Mercado Libre
    - Netflix
    - Facebook

3. **¿Qué es una página web estática? Mencione sus características**
Una página web estática es un tipo de sitio web cuyos contenidos se muestran de la misma forma para todos los usuarios y no cambian a menos que un desarrollador edite manualmente su código fuente

    **Características principales de las páginas web estáticas:**
    - **Contenido fijo:** Todos los visitantes ven exactamente la misma información, imágenes y diseño.
    - **Desarrollo simple:** Se construyen mayoritariamente con HTML y CSS, facilitando su creación y alojamiento.
    - **Alta velocidad de carga:** Al ser archivos planos y ligeros, se cargan rápidamente al no depender de consultas a bases de datos.
    - **Seguridad:** Tienen un riesgo menor de vulnerabilidades, ya que no procesan datos del usuario ni tienen un backend complejo.
    - **Interactividad limitada:** Generalmente, la interacción se reduce a enlaces y formularios básicos.
    - **Actualización manual:** Cualquier cambio en el contenido requiere modificar el archivo .html directamente.

4. **Nombre 3 ejemplos de ellas**
    - Portafolios profesionales
    - Páginas de destino
    - Páginas corporativas básicas

5. **En la actualidad, en qué caso utilizaría cada una de ellas**
Las páginas estáticas son ideales para sitios informativos, rápidos y seguros con contenido fijo (landing pages, portafolios), mientras que las dinámicas son necesarias para sitios con contenido actualizado frecuentemente, interacción de usuario o gestión de bases de datos (tiendas online, redes sociales).

## Instalación
1. **¿Qué aplicación utilizaron para instalar el servidor Web? Y ¿Por qué?**
Se elige XAMPP porque es una herramienta "todo en uno" que integra de forma conjunta Apache, MySQL, PHP y Perl, lo que destaca por su "facilidad de instalación y uso" para levantar un servidor local rápidamente.

2. **¿Cómo puedo saber qué versión de PHP tengo instalado?**
Usualmente podés saberlo ejecutando el comando php -v en tu consola o creando un archivo .php con la función phpinfo(); en tu servidor local.

3. **Indique en qué directorio del servidor tengo que alojar mi sitio/sistema para poder utilizarlo/probarlo**
El directorio raíz (DocumentRoot) donde se deben alojar por defecto los proyectos es C:\xampp\htdocs.

4. **¿Qué archivo de configuración tengo que editar para mostrar/ocultar los errores en tiempo de ejecución? Y ¿Cuáles son las distintas opciones para eso?**
Esto se configura editando el archivo php.ini de tu servidor y modificando las directivas display_errors y error_reporting.

5. **¿Cuáles son las variables que debo modificar para no tener grandes sobresaltos a la hora de implementar un sistema/sitio web?**
    - max_execution_time (tiempo máximo de ejecución).
    - memory_limit (límite de memoria).
    - upload_max_filesize y post_max_size (tamaño máximo de archivos).
    - error_reporting (nivel de errores a mostrar).
