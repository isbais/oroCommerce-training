# Especificidades y Gestión de Accounts

## Tabla de Contenidos
- [Introducción](#introducción)
- [Estructura de la Organización](#estructura-de-la-organización)
- [Gestión de Accounts](#gestión-de-accounts)

## Introducción

La última entidad de customer que vamos a discutir es una **account**. Una account representa una empresa, hogar o un grupo de personas con las que haces negocios.

Una **account** acumula información de todos los canales sobre todas las actividades relacionadas con customers, customer users, customer groups, contacts y business customers asociados con la account.

Cuando creas o editas cualquier entidad de customer en el back-office, puedes especificar la account relacionada directamente. Cuando un nuevo customer se auto-registra en el storefront, una nueva account con el mismo nombre se crea automáticamente. Hemos ilustrado este ejemplo en la primera sección de la sección cuando Jerry Blackwill, un gerente de Twin Glass & Mirror, se auto-registró una cuenta en el storefront. Esta acción activó la creación del customer y account Twin Glass & Mirror en el back-office inmediatamente.

Con Twin Glass & Mirror, hemos recorrido un largo camino a través de la sección, organizando y estructurando la información proporcionada sobre el negocio. A continuación está la ilustración de la organización de muestra de Twin Glass & Mirror que hemos construido en nuestro sistema.

![Estructura de Twin Glass & Mirror](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/twin_glass_mirror_structure-1024x461.png)

Ahora vayamos y verifiquemos qué información se muestra bajo la account Twin Glass & Mirror:

1. **Navega a Customers > Accounts** en el menú principal.

![Página de Todas las Accounts](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/all_accounts_page-1024x327.png)

2. **Encuentra el registro de account requerido**. Para nuestro caso, es Twin Glass & Mirror. Usa filtros para acelerar tu búsqueda.

![Página de Account Twin Glass & Mirror](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/twin_glassmirror_account_page-1-768x360.png)

Aquí, puedes obtener información completa sobre los usuarios y negocios asociados con la account, principalmente:

- **La fecha de creación de la account** y su última actualización.
- **El monto calculado del valor de ventas de por vida de la account**. Esta métrica ayuda a predecir el beneficio potencial que tu organización puede obtener de una relación con el customer a largo plazo. El valor de ventas de por vida mide el monto total de dinero recibido del customer basado en órdenes realizadas y registradas en la aplicación Oro.
- **La sección General** muestra detalles generales de la account, como su nombre, tags, descripción y todos los contacts asignados a la account. Hemos asignado solo un contact (Albert Clark) a la account que se muestra bajo la sección Contacts con toda la información personal que puedas necesitar. Puedes asociar múltiples contacts con una account, pero solo uno puede ser el predeterminado.

  **P.S.** La account Visual Systems también mostrará a Albert Clark bajo la sección Contacts.

![Página de Account Visual Systems](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/vision_systems_account_page-1-768x273.png)

- **La sección Commerce channel** muestra toda la información recopilada sobre la account y sus customers de todos sus canales disponibles.
- Dentro de la sección, puedes seleccionar el customer requerido y verificar sus detalles generales, customer users y customer groups asignados, listas de compras abiertas, RFQs creadas y enviadas, cotizaciones recibidas, órdenes enviadas y oportunidades relacionadas. Es bastante útil tener todos los detalles acumulados en su lugar.

![Detalles del Canal de Comercio de la Account](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/account_commerce_channel_details-1-768x249.png)

Nuestra account de muestra, Twin Glass & Mirror, representa los customers del canal Commerce, mientras que otra account de muestra, Visual Systems, representa los business customers del canal Sales con información sobre los leads y oportunidades relacionados con sus business customers.

![Canal de Ventas de la Account](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/account_sales_channel-1-768x250.png)

Ten en cuenta que el número y nombres de estas secciones de canal (Commerce, Sales) dependen del número y nombres de los canales y registros de customer asignados a la account seleccionada. El tipo de canales puede variar dependiendo de tus configuraciones e integraciones. Una account puede tener múltiples canales.

![Canales de Ventas y Comercio de la Account](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/account_sales_commerce_channels-1-768x495.png)

- **En la sección Activity**, puedes ver todas las actividades relacionadas solo con la account, como archivos adjuntos, llamadas, eventos de calendario, notas, correos electrónicos o tareas (si están disponibles). Ten en cuenta que las acciones relacionadas con actividades que se realizaron a un customer o contact asignado a la account no se muestran aquí.
- **La sección Opportunities** almacena la información sobre todos los registros de oportunidad asociados con la account.
- Si hay otros detalles disponibles para la account, se muestran bajo las secciones **Marketing Activity** y **Additional Information**.

## Gestión de Accounts

El proceso de gestionar la información recopilada dentro de la account es similar a la forma en que gestionas otras entidades de customer. Principalmente, puedes:

- **Compartir la account** con otro usuario Oro haciendo clic en **Share** y proporcionando la información requerida en un formulario emergente.
- **Editar información de la account** haciendo clic en **Edit**.
- **Eliminar la account** del sistema haciendo clic en **Delete**.
- **Agregar archivos adjuntos, notas, eventos, tareas, contacts, enviar correos electrónicos, registrar llamadas y crear registros de oportunidad** bajo el menú **More Actions**.

![Gestionando Accounts desde la Página de Detalles](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/managing_accounts_from_details_page-1-768x321.png)

Adicionalmente, puedes procesar accounts desde la página All Accounts bajo **Customers > Accounts**.

Aquí, puedes ver, editar, eliminar o eliminar en masa los registros de account requeridos, agregar tags y renombrar accounts, crear una nueva account, importar y exportar registros de account en masa, etc.

![Gestionando Accounts desde la Cuadrícula](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/managing_accounts_from_grid-1-768x221.png)

También puedes fusionar múltiples accounts en una seleccionando las accounts para fusionar y haciendo clic en **Merge** en el menú de puntos suspensivos en el extremo derecho de la fila del encabezado de la tabla. Fusionar accounts es útil cuando varias accounts han sido creadas para los diferentes representantes del mismo cliente, o que tu partner business-to-business está cooperando contigo desde un nuevo canal (por ejemplo, comenzó a comprar de tu otra tienda).

![Fusionando Accounts](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/merging_accounts-1-768x251.png)

**Nota:** Para más detalles sobre cómo importar, exportar y fusionar accounts, consulta nuestra documentación en línea: https://doc.oroinc.com/user/back-office/customers/accounts/

Si quieres crear una nueva account, la única información que necesitas proporcionar es el nombre de la account y descripción. También puedes agregar los contacts requeridos y asignar el owner responsable de esta account.

![Creando Account](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/creating_account-1-768x545.png)