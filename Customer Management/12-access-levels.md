# Niveles de Acceso

## Tabla de Contenidos
- [Introducción](#introducción)
- [Niveles de Acceso en Storefront](#niveles-de-acceso-en-storefront)
- [Niveles de Acceso en Back-Office](#niveles-de-acceso-en-back-office)
- [Tipos de Niveles de Acceso](#tipos-de-niveles-de-acceso)
  - [Nivel de Acceso None](#nivel-de-acceso-none)
  - [Nivel de Acceso User](#nivel-de-acceso-user)
  - [Nivel de Acceso Department](#nivel-de-acceso-department)
  - [Nivel de Acceso Corporate](#nivel-de-acceso-corporate)
- [Gestión de Roles desde Storefront](#gestión-de-roles-desde-storefront)

## Introducción

En las aplicaciones Oro, los niveles de acceso para customer user roles son similares a los roles de usuario del back-office, pero, conceptualmente, no son los mismos.

Los roles de usuario del storefront tienen cuatro niveles de acceso: **None**, **User**, **Department** y **Corporate**.

![Niveles de Acceso en Storefront](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/access_levels_storefront-1-768x288.png)

Mientras que los roles de usuario del back-office tienen seis niveles de acceso: **None**, **User**, **Business Unit**, **Division**, **Organization** y **Global**.

![Niveles de Acceso en Back-Office](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/access_levels_back_office-1-768x321.png)

**Nota:** Como la gestión de roles de usuario del back-office no es parte de este curso, no cubriremos sus especificidades de nivel de acceso aquí, pero siempre puedes aprender más sobre ellos en nuestra documentación en línea.

## Niveles de Acceso en Storefront

Para ilustrar los cuatro niveles de acceso que pueden ser definidos para cualquier rol de usuario en el storefront, vamos a construir una estructura de muestra de Departamentos de Compras para tanto la empresa Twin Glass & Mirror como su subsidiaria Canada BU. Ambas empresas tienen Team Leaders que controlan la actividad de sus compradores en tu sitio web. Veamos qué información estará disponible para ellos si se habilita un cierto nivel de acceso para su rol.

![Organización de Empresa de Muestra](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/sample_company_organization-1024x454.png)

Como ejemplo, echemos un vistazo a la entidad **Request for Quote** bajo la pestaña **Quotes**. Los permisos aquí habilitan a un customer user a gestionar las RFQs bajo el menú de account relacionado en el storefront. Actualmente, el nivel de acceso del rol está establecido en **None**, lo que significa que no tiene permisos en absoluto. Para modificarlo, haz clic en el enlace de nivel de acceso **None** para mostrar la lista de otros niveles. Selecciona el nivel requerido para cada permiso. Repite el proceso para cada entidad que necesite ser modificada.

## Tipos de Niveles de Acceso

### Nivel de Acceso None

El nivel de acceso **None** restringe el acceso a cualquier registro, lo que significa que tales datos o acción están deshabilitados para el customer user. Si seleccionas **None** para la entidad RFQ, el customer user no podrá ver ninguna RFQ en el storefront.

### Nivel de Acceso User

El nivel **User** da acceso solo a los propios registros de un customer user. Seleccionar el nivel **User** para nuestro caso habilitará a un comprador o gerente de compras a ver solo sus propias RFQs, incluso si gestionan y controlan otros co-empleados.

![Nivel de Acceso User](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/user_access_level-1024x446.png)

### Nivel de Acceso Department

El nivel de acceso **Department** habilita a un customer user a gestionar los registros creados por otros usuarios de la empresa que pertenecen al mismo departamento. Si seleccionas este nivel de acceso para el rol Procurement TL, entonces el TL de Twin Glass & Mirror (HQ) podrá ver las RFQs creadas por todos los usuarios del mismo departamento. En nuestro caso, es Twin Glass & Mirror HQ. Los registros creados por usuarios de otros departamentos, subsidiarias o afiliadas no están disponibles ya que son elegibles solo para el acceso del departamento.

![Nivel de Acceso Department 1](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/department_access_level_1-1024x446.png)

Mientras que el gerente de la subsidiaria Canada BU podrá ver solo las RFQs creadas por usuarios asignados a este departamento.

![Nivel de Acceso Department 2](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/department_access_level_2-1024x416.png)

### Nivel de Acceso Corporate

El nivel de acceso **Corporate** otorga acceso completo dentro del customer, sus customers hijos y departamentos subsidiarios. Con este acceso, los TLs de Twin Glass & Mirror HQ están autorizados a ver las RFQs creadas por todos los usuarios de HQ, Canada BU y cualquier otro departamento asignado al customer padre.

![Nivel de Acceso Corporate 1](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/corporate_access_level_1-1024x446.png)

**Nota:** Ten en cuenta que ni el acceso **Department** ni **Corporate** otorgan a tu customer user acceso a los departamentos que están más arriba en la jerarquía de la organización. Significa que si a un gerente de la subsidiaria Canada BU se le otorgan los permisos más altos, aún no serán elegibles para ver las RFQs creadas por usuarios de la HQ.

![Nivel de Acceso Corporate 2](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/corporate_access_level_2-1024x446.png)

Con esto en mente, ahora puedes establecer los niveles de acceso y permisos necesarios a los roles que tu customer requiere.

## Gestión de Roles desde Storefront

Alternativamente, el customer user que inicialmente tiene permiso para gestionar roles puede hacerlo independientemente desde su Account en el storefront, bajo el menú **Roles**. La lógica, proceso y entidades son los mismos. La información se sincroniza, por lo que cualquier cambio hecho en el storefront se refleja en el back-office, y viceversa.

Para habilitar a customer users a gestionar roles desde el storefront, necesitas establecer los niveles de acceso apropiados a todos los permisos requeridos para la entidad **Customer User Role** bajo **Account Management**.

De esta manera, un Procurement TL, por ejemplo, puede manejar todos los roles a los que puede acceder, excepto el suyo propio. El propósito de eso es restringir al customer user de alternar sus propios permisos y prevenir que actúen fuera de su autoridad.

Sin embargo, también es posible hacer el rol auto-gestionado habilitando la opción **Self-Managed** bajo la sección **General Information**. Asegúrate de que los permisos de la entidad **Customer User Role** también estén establecidos, de lo contrario, habilitar la opción no hará ninguna diferencia.

El mismo customer user ahora es elegible para manejar sus propios roles además de otros roles a los que puede acceder.

