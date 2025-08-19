# Permisos de Roles de Customer User

## Tabla de Contenidos
- [Introducción](#introducción)
- [Tipos de Permisos](#tipos-de-permisos)
  - [Permisos a Nivel de Entidad](#permisos-a-nivel-de-entidad)
  - [Capacidades del Sistema](#capacidades-del-sistema)
  - [Permisos de Workflow](#permisos-de-workflow)
- [Niveles de Acceso](#niveles-de-acceso)

## Introducción

La capacidad de realizar ciertas acciones en tu sitio está gobernada por **permisos**. Cada permiso tiene un nombre (View, Create, Edit, Delete, Assign) y cubre una acción o un pequeño subconjunto de acciones. Siempre que otorgues permisos a un rol, puedes controlar qué puede o no puede hacer un customer user con este rol dentro de tu sitio web.

Un rol tiene los siguientes tipos de permisos:

- **Entity-level permissions** (Permisos a nivel de entidad)
- **System capabilities** (Capacidades del sistema)
- **Workflow permissions** (Permisos de workflow)

![Permisos de Roles](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/role_permissions-1-768x363.png)

## Tipos de Permisos

### Permisos a Nivel de Entidad

Estos permisos habilitan a los customer users a realizar una cierta acción en una entidad. Todas las entidades están listadas bajo la sección **All** y agrupadas bajo categorías, tales como Account Management, Catalog, Shopping, Quotes, Orders, etc.

Un ejemplo podría ser habilitar a un gerente de compras a crear, ver, editar y eliminar órdenes mientras se deshabilita la capacidad de reasignar la orden a otro gerente. Estos permisos de entidad de órdenes están ubicados bajo la sección relacionada **Orders**. Haz clic en las pestañas para encontrar la entidad requerida y establecer los permisos a ella.

![Permisos a Nivel de Entidad](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/entity_level_permissions-1-768x221.png)

### Capacidades del Sistema

Con las **system capabilities**, puedes habilitar cualquier funcionalidad del sistema dependiendo de la entidad requerida. Como estas capacidades pertenecen a todo el sistema, no requieren un conjunto separado de permisos. Pueden ser habilitadas o deshabilitadas para el rol seleccionado.

![Capacidades del Sistema](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/system_capabilities-1-768x213.png)

### Permisos de Workflow

En el storefront, los **workflows** ayudan a organizar y dirigir la actividad de los customer users (por ejemplo, durante el checkout), haciéndolos seguir pasos particulares en un orden predefinido (por ejemplo, proporcionar una dirección de envío, luego seleccionar un método de envío y términos de pago), o previniéndolos de realizar acciones que contradicen o entran en conflicto con los pasos lógicos de un proceso (por ejemplo, un customer puede no ser capaz de enviar una orden sin la aprobación de su gerente).

Con los **workflow permissions**, puedes controlar qué workflow habilitar para customer users y qué transición pueden realizar. También puedes expandir el workflow seleccionado y establecer permisos para cada paso del workflow.

**Nota:** Para más detalles sobre configuración y gestión de workflows, consulta nuestra documentación en línea: https://doc.oroinc.com/user/back-office/system/workflows/

![Permisos de Workflow](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/workflow_permissions-1024x384.png)

## Niveles de Acceso

Cada permiso, ya sea a nivel de entidad o workflow, puede ser asignado un cierto nivel de acceso. Elige la entidad o workflow al que quieres otorgar acceso específico, haz clic en el nombre del permiso (create, edit, view, delete) y selecciona el nivel de acceso requerido de la lista.

![Niveles de Acceso](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/access_levels-1-768x295.png)

