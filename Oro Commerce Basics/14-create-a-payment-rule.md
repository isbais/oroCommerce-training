# Crear una Regla de Pago

## 📋 Tabla de Contenidos

- [Introducción](#introducción)
- [Requisitos Previos](#requisitos-previos)
- [Crear una Nueva Regla de Pago](#crear-una-nueva-regla-de-pago)
- [Configurar Información General](#configurar-información-general)
- [Configurar Destinos](#configurar-destinos)
- [Configurar Métodos de Pago](#configurar-métodos-de-pago)
- [Resultado Final](#resultado-final)

---

## Introducción

En OroCommerce, las **reglas de pago** se usan para determinar y mostrar opciones de pago para un comprador. Los vendedores pueden configurar reglas de pago para un destino cierto o calificar una regla de pago relacionada con un atributo de cliente o producto usando condiciones de expresión.

Puedes configurar una o más reglas de pago que habiliten los métodos de pago para los destinos proporcionados.

## Requisitos Previos

> **Nota**: Asegúrate de que las integraciones para los métodos de pago que planeas usar (**PayPal Payflow Gateway**, **PayPal Payments Pro**, etc.) ya estén configuradas. En la lección anterior, hemos configurado una integración de término de pago, que ahora necesitamos agregar a la regla de pago.

## Crear una Nueva Regla de Pago

Para crear una nueva regla de pago:

### Pasos para Crear la Regla:

1. **Navega** a `System > Payment Rules` en el menú principal. Se abre la lista de reglas de pago.
2. **Haz clic** en `Create Payment Rule`.

## Configurar Información General

3. **En la sección General Information**:
   - **Selecciona** la casilla **Enabled** para activar la regla de pago. Puedes mantenerla desmarcada mientras estás redactando y probando las condiciones.
   - **Especifica** el nombre de la regla de pago y el orden de clasificación para establecer la prioridad comparada con otras reglas de pago.
   - **Selecciona** la moneda de pago.
   - **Selecciona** **Stop Further Rule Processing** si te gustaría prevenir aplicar otras reglas de pago con menor prioridad.

## Configurar Destinos

4. **En la sección Destinations**, agrega uno o más destinos para aplicar esta regla de pago. La regla de pago se aplica cuando la dirección de facturación coincide con el(los) destino(s) proporcionado(s). Para agregar un destino, haz clic en `+Add` (ej., selecciona un país o selecciona un país y estado; para la mayor granularidad, puedes proporcionar una lista distinta de códigos postales para aplicar la regla de pago).

   ![Crear Regla de Pago](https://hive.oroinc.com/wp-content/uploads/sites/21/2018/06/payment_rule_create-1536x750.png)

## Configurar Métodos de Pago

5. **En la sección Payment Method Configurations**, puedes habilitar uno o más métodos de pago con esta regla de pago. Para agregar un método de pago, selecciónalo de la lista y haz clic en `+Add`. Como solo tenemos un método de pago disponible, seleccionamos **net 10** de la lista.

   ![Configurar Método de Pago](https://hive.oroinc.com/wp-content/uploads/sites/21/2018/06/payment_rule_method-1536x420.png)

6. **Haz clic** en `Save and Close`.

## Resultado Final

   ![Storefront con Método de Pago](https://hive.oroinc.com/wp-content/uploads/sites/21/2018/06/PaymentStorefront2-720x443-1.jpg)

> **Nota**: La captura de pantalla es una ilustración, ya que no podrás ver realmente cómo se ve el método de pago hasta que agregues tu método de envío.

Con un método de pago creado, solo queda una cosa para permitir que los clientes procedan a través del **checkout**, y eso es un **método de envío**. De manera similar a configurar pagos en Oro, necesitas crear una integración con un **proveedor de envío** y agregarlo a una **regla de envío**.

---

*Este documento forma parte de la guía de Oro Commerce Basics.*