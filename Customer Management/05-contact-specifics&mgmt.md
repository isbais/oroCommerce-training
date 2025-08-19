# Especificidades y Gestión de Contacts

## Tabla de Contenidos
- [Introducción](#introducción)
- [Creación de Contact](#creación-de-contact)
- [Gestión de Contacts](#gestión-de-contacts)

## Introducción

En las secciones anteriores, hemos ilustrado las interacciones business-customer que principalmente ocurren a través de tu storefront del sitio web. Sin embargo, estos intercambios también pueden suceder a través de un canal de comunicación diferente, como teléfono, correo electrónico, web y texto, o redes sociales. Tales consumidores no requieren una cuenta dedicada en tu storefront. Entonces, puedes registrarlos como **contacts**.

Un **contact** representa una persona con la que te pones en contacto durante las actividades comerciales. Un registro de contact contiene información personal, como nombres y apellidos, un número de teléfono, direcciones de correo electrónico, títulos de trabajo, direcciones de envío y facturación, enlaces a redes sociales, etc. Un contact puede entonces ser asignado a un **business customer** y una **account**, si es necesario.

![Tabla de Registro de Contact](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/contact_record_table-1024x325.png)

## Creación de Contact

Para nuestro caso, creemos un contact, Sr. Albert Clark, un especialista en inspección de vidrio que proporciona evaluación de calidad de vidrio para tu empresa. Él representa a la empresa Visual Systems, uno de tus subcontratistas. Visual Systems, sin embargo, es una empresa bien conocida que proporciona servicios a múltiples organizaciones, incluyendo Twin Glass & Mirror.

Para esto:

1. **Navega a Customers > Contacts** en el menú principal.

2. **Haz clic en Create Contact** en la parte superior derecha de la página.

3. **En la sección General**, define las configuraciones básicas del contact creado, como un owner, nombres y apellidos, descripción de texto libre, correos electrónicos, números de teléfono, cumpleaños, etc.

![Creando Contact](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/creating_contact-1024x448.png)

- **En el campo opcional Assigned To**, especifica un usuario Oro que trabajará con el contact.
- **En el campo opcional Reports To**, especifica otro registro de contact existente al cual el nuevo contact reporta (por ejemplo, gerente del departamento, CEO de la empresa, etc.). Es útil tener un contact adicional a mano en caso de que tu contact usual deje su empresa, por ejemplo. Aunque no es requerido, los contacts adicionales son altamente recomendados.

![Creando Contact Parte 2](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/creating_contact_part2-1-768x301.png)

- **En el campo Picture**, agrega una foto u otra imagen identificativa para ser usada para el contact en la UI.
- **En el formulario Addresses**, define las direcciones de facturación y envío del contact. Puedes agregar un número ilimitado de direcciones para un solo contact.

4. **La sección Groups** contiene todos los contact groups disponibles en el sistema. Marca las casillas para asignar el contact a un grupo para entender mejor el rol del contact. Un contact puede ser asignado a varios grupos. Esta información puede ser usada para propósitos de reportes o notificaciones. Puedes crear nuevos grupos o editar los existentes bajo **System > Contact Groups** en el menú principal.

   **Nota:** Para más detalles sobre cómo crear nuevos contact groups y usarlos en filtros y segmentos, consulta nuestra documentación en línea: https://doc.oroinc.com/user/back-office/system/contact-groups/#contact-groups

5. **La sección Accounts** contiene todas las accounts disponibles en el sistema. Marca las casillas para asociar el contact con una account. Un contact también puede ser asignado a varias accounts. El propósito de esto es proporcionar una vista de 360 grados de un customer y registros asociados. Un contact no necesariamente tiene que estar asociado con una account, pero esto es altamente recomendado.

   En nuestro caso, Albert Clark representa a la empresa Visual Systems, y él también controla la calidad del vidrio para Twin Glass & Mirror. Para este caso, asignemos al Sr. Clark a ambas accounts. De esta manera, podemos ver qué información y cómo se mostrará en las accounts cuando lleguemos a esta sección más adelante en esta sección.

![Creando Contact Parte 3](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/creating_contact_part3-1-768x319.png)

Si no tienes una account dedicada creada, entonces deja el contact sin asignar. Puedes hacerlo en cualquier momento después de que la account sea creada.

6. **Haz clic en Save** para guardar tu nuevo contact.

## Gestión de Contacts

Ahora que has creado tu nuevo contact, puedes gestionarlo directamente desde su página de vista.

Aquí, puedes:

- Verificar toda la información personal y de contacto requerida
- Navegar a las páginas de accounts y representantes asignados
- Enviar correos electrónicos, agregar notas, eventos, tareas y registrar llamadas bajo el menú **More Actions** en la esquina superior derecha de la página
- Ver todos los intercambios escritos, llamadas registradas y cualquier otra nota bajo la sección **Activity**
- Acceder a la información agregada sobre la actividad de marketing del contact bajo las secciones relacionadas
- Actualizar los detalles del contact haciendo clic en el botón **Edit**
- Compartir los detalles del contact con otro usuario Oro haciendo clic en el botón **Share**
- Remover registros de contact innecesarios haciendo clic en el botón **Delete**

![Ver Registro de Contact](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/view_contact_record-1-768x292.png)

Adicionalmente, puedes procesar contacts desde la página All Contacts bajo **Customers > Contacts**.

Aquí, puedes:

- Ver, editar, eliminar o eliminar en masa los registros de contact requeridos haciendo clic en el ícono apropiado bajo el menú **More Options**
- Agregar tags (por ejemplo, #new, #vip, wholesalers, partners, etc.) directamente desde la cuadrícula con la ayuda de la característica de edición en línea
- Crear un nuevo contact manualmente haciendo clic en **Create Contact** en la parte superior derecha
- Importar registros de contact en masa haciendo clic en **Import file** y navegando a través de todos los pasos requeridos
- Descargar todos los registros de contact disponibles en el sistema independientemente de los filtros aplicados a la cuadrícula haciendo clic en el botón **Export**
- Exportar solo la lista de registros filtrados haciendo clic en el botón **Export Grid**

**Nota:** Para más detalles sobre cómo importar y exportar contacts, consulta nuestra documentación en línea: https://doc.oroinc.com/user/back-office/customers/contacts/

![Gestionando Tabla de Registro de Contact](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/managing_contact_record_table-1-768x229.png)
