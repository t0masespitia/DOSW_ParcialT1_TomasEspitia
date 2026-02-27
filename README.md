# DOSW_ParcialT1_TomasEspitia
#Parcial 1

**Nombre:** Tomas Espitia
**Grupo:** 2

## Punto 1 - Diagrama de contexto 
![img.png](docs/images/img.png)

---

## Punto 2 - Patrones de diseño
**Patron # 1:**
- **Nombre del Patrón:**  Abstract Factory
- **Tipo de patrón:** Creacional
- **Justificación de la decisión:**  Porque  tenemos
  que poder cambiar entre proveedores
  sin modificar el proceso de pago inicial que llevamos.

**Patron # 2:**
- **Nombre del Patrón:** Adapter
- **Tipo de patrón:** Estructural
- **Justificación de la decisión:** Porque cada proveedor
  que hay nos esta devolviendo informacion
  en distintos tipos.

---

## Punto 3 - Identificar 5 requerimientos

### Funcionales:
### 1.
Registrar Solicitud de pago: El sistema debe permitir registrat una solicitud de pago con nombre, monto, tipo de moneda.
### 2.
Procesar pago seleccionando la correspondiente: El sistema debe permitir procesar la solicitud de pago seleccionadon la correspondiente dependiendo la moneda y el medio de pago que se usara.
### 3.
Condultar el estado en el que esta la transaccion: Se debe poder ver el estado en que va la transaccion usando su codigo y nos debe devolver en que estado esta, la fecha y mensaje que tenga.
### No funcionales:
### 1.
Usar colores que sean institucionales
### 2.
Que haya un tiempo de respuesta predeterminado

---

## Punto 4 - Diagrama casos de uso

### 1.
- Como Pagador
- Quiero consultar el estado en el que esta la transaccion
- Para que el sistema seleccione el proveedor correcto y me devuelva una respuesta que lleve (estado, código, fecha, mensaje)
- En este usamos abstract factory porque se selecciona la familia del proveedor dependiento la moneda y el metodo de pago
- En este usamos adapter porque unificamos las respuestas que nos envian en diferentes formatos conviertiendolos en uno solo
![img_1.png](docs/images/img_1.png)
### 2.
- Como Pagador o Administrador
- Quiero consultar el estado de una transacción usando su código
- Para saber si esta aprobada, o la rechazaron, esta pendiente y poder ver la fecha y mensaje
![img_2.png](docs/images/img_2.png)
---







