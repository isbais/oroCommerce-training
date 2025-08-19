# Especificidades y Gestión de Business Customers

## Tabla de Contenidos
- [Introducción](#introducción)
- [Habilitación de la Funcionalidad de Business Customers](#habilitación-de-la-funcionalidad-de-business-customers)
- [Creación de Business Customer](#creación-de-business-customer)
- [Gestión de Business Customers](#gestión-de-business-customers)

## Introducción

Similarmente a los customer users, los **contacts** también son personas reales, empleados de una empresa. Sin embargo, a diferencia de los customer users, no necesitan una cuenta en tu storefront.

Podemos dibujar un paralelo entre un **customer** y un **business customer**, que representan empresas o divisiones. Mientras que los commerce customers se usan para agregar todos los usuarios relacionados con ellos, los business customers se usan principalmente para representar unidades de negocio, departamentos o divisiones que una empresa puede tener. Por ejemplo, la account Visual System puede tener múltiples departamentos (por ejemplo, administración, servicio, ventas, financiero), divisiones basadas en servicios (por ejemplo, inspección de vidrio, inspección de madera, inspecciones de acero y empaque), unidades de negocio y subsidiarias en diferentes ciudades. Si necesitas estructurar estos departamentos adecuadamente en tu sistema, puedes usar Business Customers para eso. Sin embargo, a diferencia de los commerce customers, los business customers solo pueden ser asignados un contact para representarlo. Otros contacts pueden ser conectados directamente a la account correspondiente.

## Habilitación de la Funcionalidad de Business Customers

La funcionalidad de **Business Customers** es opcional en la aplicación Oro y no está habilitada por defecto. Puedes usar Accounts en lugar de business customers, si es necesario. A través de accounts, también puedes rastrear actividades y registros asociados con ellos a través de diferentes canales. Lo veremos más adelante en la sección.

Sin embargo, si una empresa con la que haces negocios requiere una separación clara de sus divisiones, los business customers resultan útiles para eso.

Para habilitar business customers en tu aplicación Oro, debes tener los permisos apropiados activados para tu rol de back-office. Cuando todos los permisos estén en su lugar, crea un canal de ventas:

1. **Navega a System > Channels** en el menú principal.

2. **Haz clic en Create Channel**.

3. **Una vez que se abre el formulario:**

   - Proporciona un **Name** significativo para el canal (por ejemplo, Sales Channel).
   - Establece el **Channel Type** a Sales.
   - En la sección **Entities**, selecciona **Business Customer** de la lista, y haz clic en **Add**.
   - Haz clic en **Save and Close**.

![Creando Channel](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/creating_channel-1024x370.png)

4. **Una vez que el canal se guarda**, la sección **Business Customers** aparece bajo el menú Customers.

   **Nota:** Encuentra más detalles sobre channels en nuestra documentación en línea: https://doc.oroinc.com/user/back-office/system/channels/

![Sección del Menú Business Customers](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/Business_customers_menu_section-1-768x278.png)

## Creación de Business Customer

En la sección anterior, hemos creado un contact, Sr. Albert Clark, que emprende inspección de calidad de vidrio para Visual Systems.

Ahora creemos un business customer que representaría al equipo Glass Inspection Service, asociarlo con la account Visual Systems, y vincular el contact del Sr. Clark a él.

Para eso:

1. **Navega a Customers > Business Customers** en el menú principal.
2. **Haz clic en Create Business Customer** en la parte superior derecha de la página.
3. **En el campo Account**, selecciona la account a la cual se asignará el customer. Los detalles de este business customer serán entonces parte de los detalles de esta account. En nuestro caso, es Visual Systems.
4. **En el campo Owner**, selecciona el usuario cuyos roles permiten gestionar business customers asignados al owner (por ejemplo, el owner, miembros de la misma unidad de negocio, administrador del sistema, etc.). Por defecto, se elige el usuario que crea el registro.
5. **Proporciona el Customer Name** usado para referirse al business customer en el sistema. En nuestro caso, es Glass Inspection Service BU.
6. **Selecciona el Contact** que representa al business customer. En nuestro caso, asignaremos a Albert Clark como persona de contacto para Glass Inspection Service BU.
7. **Agrega un número de teléfono**, dirección de correo electrónico, direcciones de envío y facturación. Es posible agregar múltiples registros aquí, si se requiere.
8. **Adicionalmente**, puedes marcar la dirección del sitio web del business customer, el número de empleados que trabajan para el business customer, el tipo de su propiedad legal, y la calificación interna del business customer en tu aplicación.
9. **Haz clic en Save and Close** cuando termines.

![Crear Business Customer](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/create_business_customer-1-768x454.png)

## Gestión de Business Customers

Una vez que tu nuevo business customer está creado, puedes comenzar a gestionarlo directamente desde su página de vista.

Aquí, puedes:

- Verificar toda la información de contacto requerida
- Navegar a las páginas de la account y contact asignados
- Agregar tags para organizar los customers en categorías lógicas
- Enviar correos electrónicos, agregar notas, eventos, tareas y registrar llamadas bajo el menú **More Actions** en la esquina superior derecha de la página
- Ver todos los intercambios escritos, llamadas registradas y cualquier otra nota bajo la sección **Activity**
- Acceder a la información agregada sobre los leads y oportunidades bajo las secciones relacionadas
- Actualizar los detalles del contact haciendo clic en el botón **Edit**
- Remover registros de contact innecesarios haciendo clic en el botón **Delete**

![Ver Detalles de Business Customers](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/view_business_customers_details-1-768x327.png)

Adicionalmente, puedes procesar business customers desde la página All Business Customers bajo **Customers > Business Customers**.

Aquí, puedes ver, editar, eliminar o eliminar en masa los registros de business customer requeridos, agregar tags, crear un nuevo business customer, importar y exportar registros, etc.
