# 1.- ¿Qué es apache,mysql,php?

## Apache
Es el Servidor Web más utilizado, líder con el mayor número de instalaciones a nivel mundial muy por delante de otras soluciones como el IIS (Internet Information Server) de Microsoft. Apache es un proyecto de código abierto y uso gratuito, multiplataforma (hay versiones para todos los sistemas operativos más importantes), muy robusto y que destaca por su seguridad y rendimiento.
Ahora bien,se puede estar preguntando alguien, ¿qué es un Servidor Web y qué hace exactamente?

Bueno, lo primero que debemos aclarar es que estamos hablando de software, aunque el equipo donde se ejecuta recibe la misma denominación. Su misión es crítica, ya que es el encargado de aceptar las peticiones de páginas (o recursos en general) que provienen de los visitantes que acceden a nuestro sitio web y gestionar su entrega o denegación, de acuerdo a las políticas de seguridad establecidas. Esto, que puede parecer simple, implica muchas facetas y funcionalidades que debe cubrir, como pueden ser:

Atender de manera eficiente, ya que puede recibir un gran número de peticiones HTTP, incluyendo una ejecución multitarea ya que pueden darse peticiones simultáneas. Cualquier petición compleja (por ejemplo con acceso a base de datos) dejaría colapsado el servicio.
Restricciones de acceso a los ficheros que no se quieran ‘exponer’, gestión de autentificaciones de usuarios o filtrado de peticiones según el origen de éstas.
Manejar los errores por páginas no encontradas, informando al visitante y/o redirigiendo a páginas predeterminadas.
Gestión de la información a transmitir en función de su formato e informar adecuadamente al navegador que está solicitando dicho recurso.
Gestión de logs, es decir almacenar las peticiones recibidas, errores que se han producido y en general toda aquella información que puede ser registrada y analizada posteriormente para obtener las estadísticas de acceso al sitio web.
Además, Apache nos permite configurar un Hosting Virtual basado en IPs o en nombres, es decir, tener varios sitios web en un mismo equipo (por ejemplo: nombreweb1.com, nombreweb2.com,….) o como indicábamos, establecer distintos niveles de control de acceso a la información incluyendo el soporte a cifrado SSL utilizando protocolo seguro HTTPS.

A continuación, para los que quieran tener una visión más en detalle de cómo se trabaja con Apache, reproducimos la explicación del fichero de configuración de Apache 2 de nuestro curso Servidor Web Apache, elaborado por Franciso Illeras. 
[tutorial apache](http://www.digitallearning.es/curso-apache-servidor-web.html)

Razones de la popularidad de apache:
- Corre en una multitud de Sistemas Operativos, lo que lo hace prácticamente universal.
- Apache es una tecnología gratuita de código fuente abierto. El hecho de ser gratuita es importante pero no tanto como que se trate de código fuente abierto. Esto le da una transparencia a este software de manera que si queremos ver que es lo que estamos instalando como servidor , lo podemos saber, sin ningún secreto, sin ninguna puerta trasera ;).
- Apache es un servidor altamente configurable de diseño modular. 
- Es muy sencillo ampliar las capacidades del servidor Web Apache. 
- Actualmente existen muchos módulos para Apache que son adaptables a este, y están ahí para que los instalemos cuando los necesitemos. 
- Otra cosa importante es que cualquiera que posea una experiencia decente en la programación de C o Perl puede escribir un modulo para realizar una función determinada.
- Apache trabaja con gran cantidad de Perl, PHP y otros lenguajes de script. Perl destaca en el mundo del script y Apache utiliza su parte del pastel de Perl tanto con soporte CGI como con soporte mod perl. También trabaja con Java y páginas jsp. Teniendo todo el soporte que se necesita para tener páginas dinámicas.
- Apache te permite personalizar la respuesta ante los posibles errores que se puedan dar en el servidor. 
- Es posible configurar Apache para que ejecute un determinado script cuando ocurra un error en concreto.
Tiene una alta configurabilidad en la creación y gestión de logs. 
- Apache permite la creación de ficheros de log a medida del administrador, de este modo puedes tener un mayor control sobre lo que sucede en tu servidor .

## mysql
MySQL es un sistema de gestión de bases de datos relacional, multihilo y multiusuario con más de seis millones de instalaciones.1 MySQL AB —desde enero de 2008 una subsidiaria de Sun Microsystems y ésta a su vez de Oracle Corporation desde abril de 2009— desarrolla MySQL como software libre en un esquema de licenciamiento dual.

Por un lado se ofrece bajo la GNU GPL para cualquier uso compatible con esta licencia, pero para aquellas empresas que quieran incorporarlo en productos privativos deben comprar a la empresa una licencia específica que les permita este uso. Está desarrollado en su mayor parte en ANSI C.

Al contrario de proyectos como Apache, donde el software es desarrollado por una comunidad pública y los derechos de autor del código están en poder del autor individual, MySQL es patrocinado por una empresa privada, que posee el copyright de la mayor parte del código. Esto es lo que posibilita el esquema de licenciamiento anteriormente mencionado. Además de la venta de licencias privativas, la compañía ofrece soporte y servicios. Para sus operaciones contratan trabajadores alrededor del mundo que colaboran vía Internet. 

## php

PHP es un lenguaje de programación de uso general de código del lado del servidor originalmente diseñado para el desarrollo web de contenido dinámico. Fue uno de los primeros lenguajes de programación del lado del servidor que se podían incorporar directamente en el documento HTML en lugar de llamar a un archivo externo que procese los datos. El código es interpretado por un servidor web con un módulo de procesador de PHP que genera la página Web resultante. PHP ha evolucionado por lo que ahora incluye también una interfaz de línea de comandos que puede ser usada en aplicaciones gráficas independientes. Puede ser usado en la mayoría de los servidores web al igual que en casi todos los sistemas operativos y plataformas sin ningún costo.

Se considera uno de los lenguajes más flexibles, potentes y de alto rendimiento conocidos hasta el día de hoy. Lo que ha atraído el interés de múltiples sitios con gran demanda de tráfico como Facebook, para optar por PHP como tecnología de servidor.

# 2.- ¿Qué es lamp,wamp,mamp?

En mas de una ocasión nos hemos liado a la hora de saber cual de estos paquetes informáticos tenemos que utilizar, pues bien, aquí y ahora, de manera sencillita explicado lo que es y para que sirve cada uno:


XAMPP:  Es un servidor independiente de software libre que consiste principalmente en la base de datos MySQL, el servidor web Apache y los intérpretes para lenguajes de script: PHP y Perl. El nombre proviene del acrónimo de X (para cualquiera de los diferentes sistemas operativos), Apache, MySQL, PHP, Perl.
El programa está liberado bajo la licencia GNU y actúa como un servidor web libre, fácil de usar y capaz de interpretar páginas dinámicas. Actualmente XAMPP está disponible para Microsoft Windows, GNU/Linux, Solaris y MacOS X.

MAMP: El acrónimo MAMP se refiere al conjunto de programas software comúnmente usados para desarrollar sitios web dinámicos sobre sistemas operativos Apple Macintosh, MAC OS X. Este nombre proviene de las iniciales Mac Os X, como sistema operativo. Apache, como servidor web. MySQL sistema gestor de Bases de Datos y PHP, Perl o Python, lenguajes de programación usados para la creación de sitios web.

LAMP: Es el acrónimo utilizado para describir un sistema de infraestructura de internet que usa las siguientes herramientas: LINUX como sistema operativo, APACHE como servidor web, MySQL como gestor de base de datos y Perl, PHP o Pytho como lenguajes de programación.

WAMP: Este el acrónimo usado para describir un sistema de infraestructura de internet que usa las siguientes herramientas: WINDOWS como sistema operativo, APACHE como servidor web, MySQL como servidor web y PHP, Perl o Python como lenguajes de programación.

# 3.- Enumera lenguajes de programación para desarrollar webs

Actualmente existen diferentes lenguajes de programación para desarrollar en la web, estos han ido surgiendo debido a las tendencias y necesidades de las plataformas.

- Lenguaje HTML
Es un lenguaje estático para el desarrollo de sitios web (acrónimo en inglés de HyperText Markup Language

- Lenguaje Javascript
Este es un lenguaje interpretado, no requiere compilación.

- Lenguaje PHP

- Lenguaje ASP

- Lenguaje ASP.NET

- Lenguaje JSP

- Lenguaje Python

- Lenguaje Ruby

# 4.- Requisitos mínimos de un ordenador para instalar Ubuntu Server versiones 9.10.12.14.
