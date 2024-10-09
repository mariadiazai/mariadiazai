# Despliegue de la aplicación PokeDex en Azure 

##Requisitos previos

Antes de comenzar, asegúrate de tener lo siguiente:
- Cuenta activa de Azure for Students
. Git instalado en tu máquina.
- La aplicación PokeDex lista en tu repositorio GitHub o localmente.
- Azure CLI instalado en tu máquina.

### Paso 1: Crear un nuevo recurso en Azure

1. Inicia sesión en tu cuenta de Azure for Students desde el portal Azure Portal.
2. En el menú de la izquierda, selecciona Recursos y luego haz clic en + Crear un recurso.
3. Busca App Service y selecciónalo.
4. Configura tu App Service:
- Nombre de la aplicación: Dale un nombre único a tu aplicación (ejemplo: PokeDexApp).
- Sistema operativo: Selecciona Linux.
- Región: Selecciona una región cercana a tus usuarios principales.
- Plan de tarifa: Selecciona el plan gratuito de Azure for Students, que te permite desplegar aplicaciones web.
5. Haz clic en Revisar + Crear y luego en Crear para desplegar el recurso.

#### Paso 2: Desplegar la aplicación desde Azure 
- Nos dirigimos al recurso
- Vamos a la seccion de herramientas de desarrollo, dentro de este a herramientas avanzadas y le damos clic en ir
- Presionamos en Debug console>CMD
- Le damos clic en las carpetas site>wwwroot y en esta desplegamos, subiendo los archivos del dist en esta 
- Despues de esto funcionara la aplicacion

##### Paso 3: Verificar el despliegue

- Una vez que la aplicación se haya desplegado, puedes verificar si todo funciona correctamente visitando la URL asignada a tu aplicación en Azure.
Pero tendra problemas de seguridad en los encabezados de los headers 

###### Paso 4: Configuraramos la seguridad
- Creamos un archivo llamado web.config
- Le agregamos las directivas para seguridad 
- Observamos bien que no se haya afectado los estilos de las aplicación
- Revisamos en la pagina https://securityheaders.com/ colocamos el enlace de la aplicación


