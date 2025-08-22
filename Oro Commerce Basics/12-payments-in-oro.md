# Pagos en OroCommerce

## 📋 Tabla de Contenidos

- [Introducción](#introducción)
- [Experiencia de Compra Altamente Personalizada](#experiencia-de-compra-altamente-personalizada)
- [Diversidad de Opciones de Pago de eCommerce B2B](#diversidad-de-opciones-de-pago-de-ecommerce-b2b)
- [Líneas de Crédito y Net Terms Flexibles](#líneas-de-crédito-y-net-terms-flexibles)
- [Seguridad de Pago](#seguridad-de-pago)
- [Aprobación de Pago](#aprobación-de-pago)
- [Soluciones de OroCommerce](#soluciones-de-orocommerce)
- [Crear una Integración de Pago](#crear-una-integración-de-pago)
- [Configurar Ubicación del Comerciante](#configurar-ubicación-del-comerciante)

---

## Introducción

En el mundo donde los límites entre los modelos de negocio **B2B** y **B2C** se desdibujan, las empresas B2B frecuentemente imitan las mejores prácticas B2C. Sin embargo, no todas las estrategias que funcionan bien en **eCommerce B2C** se ajustan al entorno B2B. Los pagos son un ejemplo principal.

## Experiencia de Compra Altamente Personalizada

No hay dos negocios iguales; tampoco lo son los clientes empresariales. En **B2B**, los vendedores deben llevar la personalización al siguiente nivel, ya que cada comprador representa una pieza más grande del pastel de ingresos. Es inusual que los compradores empresariales paguen por sus compras instantáneamente. Cada comprador tiene requisitos de pago específicos y precios negociados. Sus operaciones internas pueden requerir diferentes **net terms** o el uso de soluciones de pago específicas por razones de política interna o seguridad. El desafío para el vendedor B2B es facilitar el proceso de negociación de precios y términos estableciendo reglas de pago internas para **net terms** permitidos, descuentos y opciones de pago dependiendo del volumen de pedido, margen del producto, perfil del cliente, etc., y asegurarse de que su sistema de **eCommerce B2B** sea lo suficientemente flexible para permitir reglas personalizadas para cada comprador.

## Diversidad de Opciones de Pago de eCommerce B2B

En un mundo **B2C**, un conjunto bastante limitado de opciones de pago satisface las necesidades del consumidor. Muy a menudo, una opción de tarjeta de crédito es suficiente. El **eCommerce B2B**, con sus procesos de transacción complejos y totales de pedido grandes, debe ofrecer a los clientes una gran cantidad de métodos de pago incluyendo cheques y giros postales, tarjetas de débito y crédito, así como **PayPal** u otros servicios de bóveda de pago. Puedes leer sobre los [métodos de pago](https://doc.oroinc.com/user/concept-guides/payment-configuration/) soportados por OroCommerce en la biblioteca de documentación de Oro.

## Líneas de Crédito y Net Terms Flexibles

Los clientes **B2B** están acostumbrados a hacer compras en un término de crédito negociado con el monto neto a ser pagado al vendedor dentro de un período de tiempo acordado, como 30 o 60 días. Proporcionar a los compradores términos de pago flexibles no es opcional, sino esencial para preservar tu ventaja competitiva. Competir solo en precio y gama de productos ya no es suficiente para mantenerse en la cima. Los términos de pago personalizables mejoran la lealtad del cliente. Pero ofrecer opciones de pago retrasado viene con ciertos riesgos financieros. Para estar seguros, los comerciantes usualmente buscan un proveedor de servicios de pago externo para asumir el riesgo de crédito y fraude y manejar los pagos de clientes por ellos.

## Seguridad de Pago

Debido a la frecuencia y alto valor de las transacciones **B2B**, la seguridad de datos incomprometida de los pagos en línea B2B es crítica. La pérdida de datos de pago sensibles puede llevar a pérdidas financieras colosales. Un servicio de pago en línea que use datos de pago encriptados fuera de la tienda web (ej., en forma de **tokens**) es una solución al problema de seguridad.

## Aprobación de Pago

Una organización compradora a menudo está representada por múltiples individuos que están involucrados en el proceso de compra **B2B**. Este proceso usualmente incluye varias etapas de aprobación operacional. Por ejemplo, un empleado puede estar a cargo de la investigación de productos y compilación de pedidos, pero no están autorizados para comprometer recursos de la empresa para el pago, y deben obtener aprobación primero. En algunos casos, diferentes departamentos dentro de la empresa compradora eligieron diferentes opciones de pago al hacer pedidos. Sin un sistema robusto que pueda no solo rastrear y guardar pedidos sino también permitir que múltiples compradores envíen pedidos para aprobación a través de departamentos, puede ser difícil domar el caos.

## Soluciones de OroCommerce

OroCommerce proporciona a los vendedores las características de **eCommerce B2B** y soluciones de pago que abordan todos estos desafíos. Múltiples listas de precios integradas, múltiples niveles de acceso, y características de solicitudes de cotización permiten al vendedor B2B mejorar y personalizar las experiencias de compra para sus clientes. La integración con las soluciones de pago B2B más populares satisface las preferencias de pago de los clientes B2B. Integra **PayPal** o **Authorize.Net** en OroCommerce, y acepta pagos sin efectivo vía tarjetas de débito y crédito, PayPal, o débito directo **SEPA** en más de 120 monedas desde una sola cuenta. Integra OroCommerce con **InfinitePay**, el sistema de pago B2B europeo, y asegura pagos retrasados completamente automatizados y garantizados en términos de cuenta abierta (para pedidos hasta 50K Euro). La integración de **Apruve** permite a los vendedores proporcionar líneas de crédito para sus compradores en los EE.UU. y recibir pagos dentro de 24 horas después de emitir la factura.

## Crear una Integración de Pago

Al enviar un pedido, el cliente puede tener varias opciones de pago para elegir. Dependen de la dirección de pago que se recopila en el **checkout**. Una vez que se proporciona la dirección, OroCommerce evalúa los métodos de pago contra las reglas de pago especiales y expone solo las opciones recomendadas para la ubicación particular y/o basadas en otros detalles del pedido. Después de que el cliente ha seleccionado el método de pago, se les solicita ingresar los detalles de pago y proceder al **checkout**.

Dependiendo del método de pago, el pago puede ser procesado inmediatamente o puede ser retrasado por el período de tiempo pre-configurado o hasta un evento particular (ej., hasta que el pedido esté listo para entrega).

Después de que se proporcionaron los detalles de pago, el vendedor puede ver el historial de pagos, y capturar el pago retrasado.

Cuando se selecciona el término de pago, el pago se considera capturado en su totalidad, y la información de pago no está disponible.

Para vincular cualquier método de pago al proceso de **checkout**, necesitas crear una integración con un servicio de pago que selecciones. Por ejemplo, para poder proporcionar **net terms** para clientes, necesitas crear una integración de términos de pago primero. Lo mismo aplica para cheques/giros postales o cualquier servicio de pago externo. Una vez que se crea la integración, y se agrega un método de pago, necesitas agregar una regla de pago para hacer esta opción de pago visible para el comprador en el **storefront**. Cuando esto se hace, el comprador puede proceder a través del **checkout**.

Antes de proceder a crear una integración de término de pago, asegúrate de que hayas seleccionado tu ubicación de comerciante. La ubicación del comerciante es una configuración de todo el sistema que se aplica a todos los sitios web.

## Configurar Ubicación del Comerciante

Para configurar la ubicación del comerciante:

1. **Navega** a `System > Configuration` en el menú principal.
2. **Selecciona** `Commerce > Payment > General` en el panel a la izquierda.
3. **Para personalizar** la ubicación del comerciante:
   - **Limpia** la casilla `Use Default` junto a la opción.
   - **Selecciona** un nuevo país de la lista.
   - Para nuestro ejemplo, hemos seleccionado **United States**.

4. **Haz clic** en `Save Settings`.

![Configuración de Ubicación del Comerciante](https://hive.oroinc.com/wp-content/uploads/sites/21/2018/06/merchant-location.png)

---

*Este documento forma parte de la guía de Oro Commerce Basics.*