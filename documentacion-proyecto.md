## I. Objetivo del Proyecto

El objetivo principal de este proyecto es crear un sistema que realice respaldos de manera automática, evitando que la información se pierda si ocurre algún problema en el servidor. 
La idea es que el sistema trabaje solo, sin depender de una persona para hacer copias manuales, y que la información esté siempre disponible cuando se necesite.

En pocas palabras, lo que buscamos es tener un sistema más seguro, más confiable y capaz de recuperarse rápidamente ante una falla.

## II. Justificación e Importancia

Este proyecto es importante porque ayuda a que la información y los servicios no se pierdan ni se detengan ante una falla, un apagón o un error del sistema. 
En una infraestructura universitaria o empresarial, la pérdida de datos puede afectar clases, trámites, investigaciones o incluso procesos administrativos completos, por lo que contar con respaldos automáticos y monitoreo constante se vuelve indispensable.

La implementación de este sistema reduce el riesgo de que todo dependa de un solo servidor (el famoso Single Point of Failure) y mejora la continuidad operacional, ya que aunque uno falle, la información sigue estando disponible gracias a los respaldos y al monitoreo. 
Grafana además permite ver el estado de los equipos en tiempo real, lo que hace más rápido detectar y solucionar fallos antes de que se vuelvan un problema mayor.

## III. Tecnologías y Conceptos Implementados

### 3.1 Tecnologías Clave Utilizadas

| Tecnología | Rol en el Proyecto |
|---|---|
| **NGINX** | Se utilizó como punto central para gestionar solicitudes y servir como Proxy Reverso. Ayuda a organizar el tráfico interno de los servicios. |
| **Grafana (Tecnología 5 con Prometheus opcional)** | Se implementó para monitorear los servidores y ver métricas en tiempo real como uso de recursos, estado del sistema y actividad general. |

> Estas dos tecnologías fueron la base principal del proyecto, ya que una gestiona el flujo de servicio (NGINX) y la otra permite observar su comportamiento (Grafana).

---

### 3.2 Conceptos Aplicados de la Materia (T1 - T6)

| Tema | Aplicación dentro del proyecto |
|---|---|
| ✅ **Monitoreo (T4 / T1)** | Grafana permite visualizar el estado de los servidores, detectar caídas y ver rendimiento del sistema. |
| ✅ **Seguridad y Disponibilidad (T5 / T1)** | Al contar con monitoreo y respaldo, se reduce el riesgo de pérdida total de información y se mejora la continuidad del servicio. |
| ⚠ **Balanceo de tráfico o Proxy (T3/T4)** | NGINX se usó como Proxy Reverso en este proyecto. En una versión ampliada puede habilitar balanceo de carga y manejo de múltiples servidores. |

---

