# DOSW_ParcialT1_TomasEspitia
#Parcial 1

**Nombre:** Tomas Espitia
**Grupo:** 2

## Punto 6 - Requerimiento asociado

**Seleccionamos el requerimiento de procesar pago seleccionando la correspondiente**

- **Epica:** El sistema nos debe permitir procesar pagos utilizando distintos proveedores externos, viendo que el proceso principal no dependa de implementaciones especificas y que las respuestas obtenidas sean entregadas todas en una.
### Tareas tecnicas:
- **Implemntar la estructura** 
Crear interfaz, definir metodos para crear los componentes de integracion.
- **Implementar adapters de cada proveedor**
crear intefaz, implementar el adapter, y traducir las respuestas externas al formato institucional.
- **logica de seleccion** 
Determinar que frabrica usa segun la oneda que este utiliznado y sus metodo de pago, asegurar el cumplimiento de reglaas de negocio
- **Volver las respuestas una sola**
Garantizar que todas las respuestas nos devulvan el estado, mensaje, fecha
