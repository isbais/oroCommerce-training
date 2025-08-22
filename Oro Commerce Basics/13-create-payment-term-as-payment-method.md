# Crear un Término de Pago como Método de Pago

## 📋 Tabla de Contenidos

- [Introducción](#introducción)
- [Tipos de Términos de Pago](#tipos-de-términos-de-pago)
- [Configuración por Cliente](#configuración-por-cliente)
- [Integraciones Soportadas](#integraciones-soportadas)
- [Habilitar Payment Terms como Integración](#habilitar-payment-terms-como-integración)
- [Crear una Integración](#crear-una-integración)

---

## Introducción

En OroCommerce, los **términos de pago** son un conjunto de condiciones requeridas para que una venta esté completa. Esto, por ejemplo, puede ser un **net term**, que es un período de tiempo permitido para que un cliente pague el monto adeudado. Puede ser **net 10**, **30**, o **90 días** y significaría que el pago vence dentro de esos números de días después de que se compra el artículo. Otros términos de pago pueden incluir adelanto en efectivo, efectivo contra entrega, tarjetas de crédito, o aplicaciones de pago autorizadas como **PayPal**, etc.

## Configuración por Cliente

Los términos de pago pueden ser configurados por cliente, permitiéndoles usar las condiciones de pago garantizadas por su contrato con el vendedor. Los **Default Payment Terms** pueden ser configurados para grupos de clientes así como individualmente para clientes.

## Integraciones Soportadas

Para habilitar diferentes términos de pago, se deben agregar nuevos registros de integración, como se mencionó en la lección anterior. Fuera de la caja, OroCommerce soporta:

1. **Basic Payment terms**
2. **Check/Money order**
3. **PayPal systems**

En esta sección, vamos a mostrarte cómo:

1. **Habilitar Payment Terms como una Integración**
2. **Crear un Payment Term**

Para permitir que los usuarios entren al **checkout**, debe haber al menos un método de pago agregado al sistema. Sin un método de pago disponible, el comprador puede recibir un mensaje de error y puede necesitar contactar físicamente al vendedor para completar la compra. Una vez que se crea el método de pago, necesitas crear una regla de pago para vincular el método a un cliente específico.

Puedes crear tantas nuevas integraciones como necesites para que cada término de pago esté disponible para los clientes en el **checkout**.

## Habilitar Payment Terms como Integración

Para habilitar el pago como una integración:

### Pasos para Crear la Integración:

1. **Navega** a `System > Integrations > Manage Integrations` en el menú principal.
2. **Haz clic** en `Create Integration` en la parte superior derecha.
3. **En la sección Basic Information** proporciona los siguientes detalles:

   - **Type** — El tipo de integración que estás creando. Selecciona `Payment Term`.
   - **Name** — El nombre del método de pago que se muestra como una opción para la configuración de pago en la consola de administración de OroCommerce. Para nuestro ejemplo, estamos creando un término de pago **Net 10**.
   - **Label** — El nombre/etiqueta del método de pago que se muestra como una opción de pago para el comprador en el **storefront** de OroCommerce durante el **checkout**. Puede no incluir el nombre del procesador de pago, si quieres ocultarlo de los compradores. Por ejemplo, puedes ingresar **'Credit Card Payments'** si tienes un solo método de pago configurado para procesar tarjetas de crédito. Haz clic en el ícono **Translations** para proporcionar ortografía para diferentes idiomas. Haz clic en el ícono **Default Language** para volver a la vista de un solo idioma.
   - **Short label** — El nombre/etiqueta del método de pago que se muestra en los detalles del pedido en la **Consola de Administración** de OroCommerce y **storefront** después de que se envía el pedido. Haz clic en el ícono **Translations** para proporcionar ortografía para diferentes idiomas. Haz clic en el ícono **Default Language** para volver a la vista de un solo idioma.
   - **Status** — Establece el estado en **Active** para habilitar la integración.
   - **Default Owner** — Un usuario que es responsable de esta integración y la gestiona.

4. **Establece** el estado en **Active** para habilitar la integración.
5. **Haz clic** en `Save and Close`.

![Configuración de Payment Term](https://hive.oroinc.com/wp-content/uploads/sites/21/2018/06/payment-term.png)

## Crear una Integración

> **Nota**: Cuando usas términos de pago como una integración, tienes la opción de notar términos específicos y luego asignarlos a un cliente o un grupo de clientes para que esa información se muestre al cliente durante el **checkout**. Puedes crear tales términos de pago bajo `Sales > Payment Terms` en el menú principal, y luego agregar este término de pago al cliente seleccionado bajo `Customers > Customers/Customer Groups`.

Para hacer este término de pago disponible para el cliente en el **storefront**, ahora necesitamos crear una regla de pago y agregar este método de pago a ella.

---

*Este documento forma parte de la guía de Oro Commerce Basics.*