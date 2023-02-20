# Implementación de un sistema de seguridad para una empresa.
### Anteproyecto para 2ºASIR creado por: Ángel Moreno Márquez 2ºASIR I.E.S Romero Vargas.

## Introducción

En la mayoría de las empresas que se dedidan al trato de información clasificada y privada, suelen tener una red interna en la que normalmente no tienen conexión a internet directamente para evitar posibles intrusiones en la red, ya que el robo de la información privada no solamente afectará a la persona de cuya información fue robada, sino también a la empresa con multas por fallar en la clausula de protección de datos de esa información.

Es por ello que antes de realizar el trabajo de almacenar información en una empresa, es de vital importancia conocer y adaptar la seguridad para evitar la filtración de información sensible, sufrir de 'hacking' o cualquier manera de 'cracking'.

![imagen de servidor-cliente](https://psp.codeandcoke.com/_media/apuntes:clienteservidor.jpg)

## Objetivo y finalidad del proyecto

El objetivo de este proyecto tratará de crear un Servidor en Windows Server 2019 que salga a internet (con uso de DHCP y DNS) para que los ordenadores de la empresa que están conectados desde una red interna tengan conexión a internet con el mayor nivel de seguridad posible, con la creación de un servidor HTTP que estará en otro lugar que no sea la empresa en la cuales los trabajadores podrán acceder o los técnicos de la empresa para consultar la base de datos que también incluiremos en ella. A todo esto, se incluirá un protocolo de seguridad a seguir tanto para el administrador de sistemas como para los propios empreados de la empresa para evitar la fuga de información o 'cracking'.

Se pueden diferenciar dos tipos de empleados, el que trabajará a remoto (la empresa le proporcionará un portátil con un acceso por VPN) y el que trabajará fisicamente en la empresa con el ordenador de la empresa, pero ambos obtendrán el acceso al servidor HTTP.

La finalidad es dar a entender y enseñar la importancia de tener un protocolo de seguridad porque una vez que un usuario tenga un ordenador, siempre estará expuesto a un ataque cibernético y si es una empresa será un objetivo aún más a perseguir. Este modelo se puede implementar tanto en un servidor local como en cloud (tanto núbe pública, privada o híbrida, ya que por ejemplo podría ser implementado en Azure que es el servicio de Active Directory en la nube de Microsoft).

![imagen de Azure](https://upload.wikimedia.org/wikipedia/commons/thumb/a/a8/Microsoft_Azure_Logo.svg/2560px-Microsoft_Azure_Logo.svg.png)

## Medios

Para este proyecto seguiremos los siguientes pasos con el software / configuración que se explican a continuación:

+ Realizar un análisis de riesgos: Realizar un análisis de riesgos para identificar las posibles vulnerabilidades y riesgos asociados con el servidor Windows Server y los ordenadores clientes, tanto desde el punto de vista físico como lógico para identificar las posibles amenazas, como virus, malware, ataques de fuerza bruta, phishing, entre otros. Todo esto se haría con herramientas como Nessus o OpenVAS (ejemplos).

+ Políticas de seguridad: Establecer políticas de seguridad para la gestión de contraseñas, el control de acceso, la actualización de software y la monitorización de la red. Todas las políticas estarán documentadas el personal de la empresa las conocerá y podrá seguir sin problemas.

+ Firewall: Configurar el firewall para bloquear todo el tráfico no autorizado y permitir solo el tráfico necesario. 

+ Implementar un sistema de detección de intrusos (IDS) o de prevención de intrusos (IPS) para monitorizar la red y detectar posibles ataques.

+ Antivirus y anti-malware con el que se actualizará de manera automática.

+ Acceso remoto: Los empleados se podrán conectar mediante protocolos SSL/TLS, VPN o Microsoft DirectAccess.

+ Gestión de usuarios y contraseñas: Utilizar contraseñas fuertes y que se tengan que cambiar cada cierto tiempo.

+ Copias de seguridad automáticas y de forma periódica.

+ Pruebas y auditorías: Realizaré pruebas periódicas de seguridad para detectar vulnerabilidades y verificar que todas las políticas de seguridad funcionan correctamente.

+ Comprobar mediante comandos como netstat o software como NetLimiter o Wireshark (ejemplo) el consumo del ancho de red, y el tráfico de red por si hay alguna anomalía.


## Planificación 

+ 1.- Primera semana (3 Abril - 10 abril) : Desarrollo de los protocolos a seguir para el servidor de Windows Server para los técnicos de sistema y guía práctica de la utilización de los recursos de la empresa y seguridad básica para los empleados.

+ 2.- Sgunda y tercera semana (10 Abril - 24 Abril) : Creación de las máquinas virtuales, instalación y configuración de un servidor de Windows Server junto a los clientes que usarán los empleados, el servidor HTTP con una base de datos, y la conexión a remoto para los usuarios que trabajen a remoto.

+ 3.- Cuarta semana (24 Abril - 5 Mayo) : Configuración de seguridad.

+ 4.- Quinta semana (8 Mayo - 15 Mayo) : Auditorias y pruebas de seguridad

+ 5.- Mejoras en el proyecto (15 Mayo - último día de entrega).









