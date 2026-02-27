# DOSW_ParcialT1_TomasEspitia

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







