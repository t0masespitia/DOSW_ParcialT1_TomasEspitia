# DOSW_ParcialT1_TomasEspitia

**Nombre:** Tomas Espitia
**Grupo:** 2

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
- 

![img_2.png](docs/images/img_2.png)

---







