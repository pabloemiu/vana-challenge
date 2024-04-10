# Challenge Vana

Este ejercicio tiene como objetivo evaluar su capacidad para diseñar y configurar una
solución de API en la nube de AWS, así como establecer un flujo de CI/CD utilizando GitHub
Actions para una implementación eficiente y controlada.

### Pre-requisitos 📋

Para realizar esta prueba técnica necesitará:

- Cuenta de AWS Free Tier
- Cuenta de GitHub

## Comenzando 🚀

_Es necesario realizar las siguientes acciones_

_-Ir a :gear: **Settings** -> **Secrets and variables** -> **Actions** y agregar en **Repository secrets** las siguientes variables de entorno_

      AWS_ACCESS_KEY_ID
      AWS_SECRET_ACCESS_KEY

## Deployar con cloudformation el template para crear la infraestructura

\_ Iniciar con las credenciales de AWS a https://aws.amazon.com/es/console/

\_ Ir al servicio de AWS CloudFormation

\_ Estando en CloudFormation ir a la pagina **Create stack**, una vez posicionado seleccionar **Template is ready**, y luego **Upload a template file**

\_ Elige el template creado en **Choose file**, luego **Next**

\_ **Specify stack details**

\_ En esta pagina solo se debera crear un nombre al stack en **name stack**, y luego next

\_ Pagina de opciones no editar ninguna e ir a next

\_ Revisar lo cargado en la pagina **Review** y , si esta todo correcto crear el stack con el boton de **Create**

El stack entrara en progress hasta se cree correctamente cony quede en el estado CREATE_COMPLETE, de lo contrario aparecera un error que no se pudo crear el mismo

Para visualizar que los servicios se hayan creado ir a:

- aws.amazon.com/cloudformation/: Aqui se visualizara el stack creado
- aws.amazon.com/lambda/: Aqui se visualizara la lambda creada
- aws.amazon.com/iam: Ir a la pestaña **Roles** para verificar que el rol del Template ha sido creado correctamente

Para comprobar que se haya levatado satifactoriamente ir a aws.amazon.com/cloudformation/. Selecionar en stack creado y luego ir a la pestaña **Outputs** ahi se vera la URL generada para visualizar en un navegador
