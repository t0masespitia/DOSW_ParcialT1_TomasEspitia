# DOSW_ParcialT1_TomasEspitia
#Parcial 1

**Nombre:** Tomas Espitia
**Grupo:** 2

## Punto 5 - Especificar los 2 requerimientos funcionales

### 1.
- **Procesar pago seleccionando la correspondiente**
- **Descripción:** El sistema debe permitir procesar una solicitud de pago seleccionando 
el proveedor correspondiente dependiendo de la moneda y el medio de pago utilizados, y 
debe devolver una respuesta con: estado, codigo de transacción, mensaje y fecha.
- **Como la vamos a ejecutar:** El pagador ingresa los datos del pago y confirma la operacion. 
El sistema valida las reglas de negocio, selecciona el proveedor adecuado segun moneda y medio 
de pago, procesa la transacción y devuelve la respuesta en formato institucional.
- **Actor principal:** Pagador
- **Precondiciones:** El correo debe ser institucional,
El monto debe ser mayor a 5000 COP, Si la moneda es USD el proveedor permitido es Stripe,
  Si el medio de pago es PSE, el proveedor permitido es BancoPSE,

### Datos de entrada
- | Nombre              | Descripción                 | Tipo de campo  | Reglas / Aplicación           | Obligatorio |
  | ------------------- | --------------------------- | -------------- | ----------------------------- | ----------- |
  | nombrePagador       | Nombre completo del pagador | Texto          | No vacío                      | Sí          |
  | documento           | Documento del pagador       | Texto/Numérico | No vacío                      | Sí          |
  | correoInstitucional | Correo del pagador          | Texto          | Debe ser institucional        | Sí          |
  | conceptoPago        | Concepto del pago           | Texto          | No vacío                      | Sí          |
  | monto               | Valor del pago              | Numérico       | Mayor a 5000 COP              | Sí          |
  | moneda              | Moneda del pago             | Enum           | COP o USD                     | Sí          |
  | medioPago           | Medio de pago               | Enum           | TARJETA / PSE / TRANSFERENCIA | Sí          |
### Datos de salida
- | Nombre            | Descripción                       | Tipo de campo | Reglas / Aplicación              | Obligatorio |
  | ----------------- | --------------------------------- | ------------- | -------------------------------- | ----------- |
  | estado            | Resultado de la transacción       | Enum          | APROBADO / RECHAZADO / PENDIENTE | Sí          |
  | codigoTransaccion | Código único de la transacción    | Texto         | Único                            | Sí          |
  | mensaje           | Mensaje descriptivo del resultado | Texto         | Claro para el usuario            | Sí          |
  | fecha             | Fecha y hora del resultado        | Fecha         | Formato estándar                 | Sí          |


### 2.
...