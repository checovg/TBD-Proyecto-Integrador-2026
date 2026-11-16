# TBD-Proyecto-Integrador-2026
Instrucciones y recursos del proyecto integrador de Taller de Bases de Datos

Buen día.

Como parte del Proyecto Integrador de Taller de Bases de Datos, se pone a su disposición una máquina virtual con los servicios necesarios para desarrollar, publicar y probar sus aplicaciones web.

Cada alumno deberá descargar una copia de la máquina virtual e importarla en su propio equipo mediante un software de virtualización compatible.

La finalidad es que dispongan de un entorno independiente donde puedan publicar su aplicación, ejecutar sus scripts SQL y comprobar el funcionamiento de la conexión entre PHP y MariaDB.

1. Descarga de la máquina virtual

Google Drive: https://drive.google.com/file/d/1zGsZKdwxGGxXjrJzaB25hYS1ELEVgUgJ/view?usp=sharing

Descargar máquina virtual Debian 13 (OVA)

El archivo se encuentra compartido con permisos de lectura y descarga.

Consideraciones:

Descargar el archivo .ova en su equipo.

Importarlo mediante VMware Workstation u otro virtualizador compatible con el formato OVA.

Conservar una copia original para poder restaurar el entorno en caso de ser necesario.

2. Características del servidor

Sistema operativo: Debian 13, 64 bits

Servidor web: Apache

Lenguaje de programación: PHP 8.4

Motor de base de datos: MariaDB 11.8.6

Servicio de transferencia: FTP

Configuración de red: Adaptador en modo puente (Bridge)

Credenciales de acceso

La máquina virtual cuenta con usuarios previamente configurados para los servicios correspondientes.

Las credenciales de acceso a MariaDB y FTP serán proporcionadas mediante un canal institucional.

Estas credenciales son exclusivamente para el entorno de laboratorio y no deberán utilizarse en servidores de producción.

3. Indicaciones para utilizar la máquina virtual

3.1 Importación

Descargar e importar la máquina virtual en el virtualizador de su equipo.

Verificar que los recursos asignados permitan iniciar correctamente Debian 13.

3.2 Configuración de red

La máquina virtual está preparada para utilizar un adaptador de red en modo puente (Bridged).

Deberán verificar que la interfaz de red tenga una dirección IP válida dentro de su red local.

Para consultar las direcciones IP desde Debian, pueden ejecutar:

hostname -I

Importante: La dirección IP dependerá de la red a la que esté conectado el equipo donde se ejecute la máquina virtual.

3.3 Acceso a la página web

Una vez encendida la máquina virtual, abrir un navegador desde su computadora y acceder mediante:

http://IP_DE_LA_VM/

Sustituir IP_DE_LA_VM por la dirección IP correspondiente.

Deberá mostrarse la página de prueba del servidor Apache/PHP.

3.4 Publicación de archivos mediante FTP

Utilizando FileZilla u otro cliente FTP, deberán establecer una conexión con la dirección IP de su máquina virtual y las credenciales proporcionadas.

Los archivos del aplicativo deberán colocarse en el directorio de publicación configurado.

Después de transferirlos, deberán comprobar su funcionamiento desde el navegador web.

3.5 Base de datos

Utilizando las credenciales de MariaDB proporcionadas, deberán:

Importar sus scripts SQL.

Crear las tablas y relaciones necesarias.

Verificar la estructura de su base de datos.

Comprobar que su aplicativo web puede consultar, insertar, actualizar y eliminar registros, según los requerimientos establecidos.

Cuando PHP y MariaDB se ejecuten dentro de la misma máquina virtual, podrán utilizar localhost como servidor de base de datos.

No es necesario habilitar el acceso remoto a MariaDB para la comunicación local entre PHP y el motor de base de datos.

4. Consideraciones generales

La máquina virtual se proporciona con los servicios necesarios para realizar las pruebas. No contiene el proyecto desarrollado por cada alumno.

Cada estudiante será responsable de investigar su funcionamiento, importar sus scripts, publicar sus archivos y resolver los problemas de configuración que se presenten.

Las modificaciones realizadas dentro de su máquina virtual local no afectan el trabajo de sus compañeros.

El código fuente, los scripts SQL y los avances correspondientes deberán continuar registrándose en el repositorio individual de GitHub de cada alumno.

La máquina virtual no sustituye las entregas de código y documentación solicitadas.

La entrega final y la demostración se realizarán conforme al calendario establecido.

5. Seguimiento de avances en GitHub

Cada alumno deberá mantener actualizado su repositorio individual de GitHub.

Se revisará el historial de cambios (commits) para verificar el seguimiento y la evolución del proyecto.

Se recomienda que cada commit incluya un mensaje descriptivo de los cambios realizados.

El repositorio deberá conservar los archivos necesarios para revisar el trabajo desarrollado y sus avances correspondientes.
